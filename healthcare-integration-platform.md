# Healthcare Integration Platform

This is a sanitized overview of an independent Rust project built around healthcare integrations, encrypted PHI handling, and explicit service boundaries.

## What the system did

- integrated with the Elation EMR API
- synchronized patient, prescription, and lab-result data
- managed access-token retrieval, refresh, and scoped internal exposure
- separated external integration concerns from internal application and storage layers

## Representative flow

```text
Elation EMR API
  -> sync worker
  -> validation and normalization
  -> encrypted persistence for PHI fields
  -> internal services
     -> redacted read path by default
     -> decrypt-on-read only for authorized surfaces
```

In practice, that meant a background sync job could ingest external records without turning the rest of the application into a broad plaintext data surface. Sensitive fields were encrypted before persistence, and internal consumers only got decrypted values through narrow authorized paths.

## Architecture

The project was a multi-crate Rust workspace with dedicated pieces for:
- web serving
- token management
- EMR synchronization
- auth and RPC
- core domain libraries

The important part was not crate count by itself. It was keeping trust boundaries explicit so external EMR behavior, internal services, and storage concerns did not collapse into one layer.

## Sensitive data handling

- AES-256-GCM encryption and decryption for PHI fields
- encrypted storage on create and update paths
- controlled decrypt-on-read surfaces instead of broad plaintext access
- Redis-backed caching flows for patient-name lookup data and EMR access tokens

## Operational flows

- scheduled synchronization for patient, prescription, and lab-result ingestion
- token expiration and refresh handling
- cache repopulation and scoped service exposure
- controlled data movement between integration, application, and storage boundaries

## What this was proving

- sensitive external data could move through the system without flattening service boundaries
- token lifecycle work stayed isolated from business logic that only needed scoped access
- encrypted-at-rest storage and decrypt-on-read access were implementation defaults, not optional conventions

## Why this is sanitized

This writeup leaves out proprietary schema details, identifiers, and deployment specifics. The goal is to show the system shape and technical decisions that matter for evaluating the work.

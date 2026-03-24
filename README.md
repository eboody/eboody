# Hi, I'm Eran

I'm a Rust-first software engineer focused on security-sensitive data flows, system invariants, and boundary enforcement.

This profile is meant to reflect the work I'm strongest at:
- healthcare integrations against the Elation EMR API
- AES-256-GCM encryption for PHI fields
- multi-service Rust systems with explicit trust boundaries
- compile-time safety, typestate, and API-shape design

## Resume-backed systems work

### Healthcare Integration Platform

I built a multi-crate Rust workspace with dedicated web, token, sync, auth, RPC, and core domain layers. The system included:
- Elation EMR integration and scheduled synchronization for patient, prescription, and lab-result data
- AES-256-GCM encryption and decryption for PHI fields, with encrypted storage on write paths and controlled decrypt-on-read surfaces
- Redis-backed caching for patient-name lookups and EMR access tokens, including refresh scheduling and expiration handling
- explicit service boundaries between external EMR integration, internal services, and storage layers

### Production Systems

At GoodUnited, I built systems that:
- increased fundraiser acknowledgment throughput by roughly 12x per operator
- scaled to 72 concurrent workers
- replaced a manual CSV process lagging by 48 hours with realtime fundraiser creation and donation visibility
- supported products used by large national nonprofits

## Public Rust work

- [`statum`](https://github.com/eboody/statum): typestate framework for legal state transitions and rebuilding typed workflow state from persisted data.
- [`eran.codes`](https://github.com/eboody/eran.codes): public Rust reference app for layered architecture, persistence-backed auth, runtime visibility, and inspectable operational behavior.
- [`modum`](https://github.com/eboody/modum): workspace lint tool for consistent module naming, import style, and public API paths.
- [`nestum`](https://github.com/eboody/nestum): proc macro for nested enum paths that keeps structured state readable without flattening it away.
- [`maud-extensions`](https://github.com/eboody/maud-extensions): proc macros for Maud components with inline CSS, JS, slots, and font helpers.

## What I try to make true in code

- boundaries are explicit
- invalid paths do not look like valid API usage
- security properties are enforced structurally, not socially
- runtime behavior is visible enough to inspect, debug, and trust

## Links

- Website: [eran.codes](https://eran.codes)
- GitHub: [@eboody](https://github.com/eboody)
- LinkedIn: [Eran Boodnero](https://www.linkedin.com/in/eran-boodnero-602a994b/)

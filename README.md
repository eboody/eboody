# Hi, I'm Eran

I'm a Rust-first software engineer working on sensitive data, clear service boundaries, and APIs that make bad states harder to represent.

## Start here

- [Healthcare integration platform case study](./healthcare-integration-platform.md): sanitized writeup of EMR sync, encrypted PHI storage, token handling, and the public `eran.codes` demo that backs it up.
- [`eran.codes`](https://github.com/eboody/eran.codes): my current public Rust reference app for layered architecture, persistence-backed auth and sessions, runtime visibility, and operational surfaces.
- [`statum`](https://github.com/eboody/statum): typestate framework for legal state transitions and rebuilding typed workflow state from persisted data.

## What I build

- healthcare integrations against the Elation EMR API
- encrypted storage for PHI fields
- Rust services with clear boundaries between external systems, app logic, and storage
- type-driven libraries focused on state and API design

## Production impact

- increased fundraiser acknowledgment throughput by roughly 12x per operator
- scaled automation to 72 concurrent workers
- replaced a manual CSV process lagging by 48 hours with realtime fundraiser creation and donation visibility
- supported products used by large national nonprofits

## More public Rust work

- [`modum`](https://github.com/eboody/modum): workspace lint tool for consistent module naming, import style, and public API paths.
- [`nestum`](https://github.com/eboody/nestum): proc macro for nested enum paths that keeps structured state readable without flattening it away.
- [`maud-extensions`](https://github.com/eboody/maud-extensions): proc macros for Maud components with inline CSS, JS, slots, and font helpers.

## What I care about

- boundaries are explicit
- risky paths do not look like normal API usage
- security rules are built into the system instead of left to convention
- runtime behavior is visible enough to inspect and debug

## Links

- Website: [eran.codes](https://eran.codes)
- GitHub: [@eboody](https://github.com/eboody)
- LinkedIn: [Eran Boodnero](https://www.linkedin.com/in/eran-boodnero-602a994b/)

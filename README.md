# Hi, I'm Eran

I'm a Rust-first software engineer focused on system boundaries, security-sensitive data flow, and invariants enforced in code.

Right now I'm using [`eran.codes`](https://github.com/eboody/eran.codes) as a public Rust reference app for:
- layered application structure
- persistence-backed auth and sessions
- runtime visibility and operational surfaces
- secure data flow and integration boundaries

## Open-source work

- [`statum`](https://github.com/eboody/statum): typestate framework for legal state transitions and rebuilding typed workflow state from persisted data.
- [`eran.codes`](https://github.com/eboody/eran.codes): my personal site and lab, built as a Rust system with explicit crate boundaries and inspectable runtime behavior.
- [`modum`](https://github.com/eboody/modum): workspace lint tool for consistent module naming, import style, and public API paths.
- [`nestum`](https://github.com/eboody/nestum): proc macro for nested enum paths that keeps structured state readable without flattening it away.
- [`maud-extensions`](https://github.com/eboody/maud-extensions): proc macros for Maud components with inline CSS, JS, slots, and font helpers.

## Systems work

I built a multi-crate Rust healthcare integration platform with separate web, token, sync, auth, RPC, and core domain layers. It handled EMR synchronization, AES-256-GCM encryption for PHI fields, Redis-backed token and lookup caching, and explicit service boundaries around sensitive data access.

I also built production automation and realtime data systems that:
- increased fundraiser acknowledgment throughput by roughly 12x per operator
- scaled to 72 concurrent workers
- replaced a 48-hour CSV lag with realtime fundraiser and donation visibility

## What I optimize for

- boundaries that are visible in the codebase
- APIs that remove illegal paths from call sites
- security properties enforced by structure instead of convention
- runtime behavior you can inspect while the system is running

## Links

- Website: [eran.codes](https://eran.codes)
- GitHub: [@eboody](https://github.com/eboody)
- LinkedIn: [Eran Boodnero](https://www.linkedin.com/in/eran-boodnero-602a994b/)

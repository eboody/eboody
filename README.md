# Hi, I'm Eran

I build Rust systems where correctness, security, and data boundaries are explicit.

Current focus: turning [`eran.codes`](https://github.com/eboody/eran.codes) into a public Rust reference app for explicit boundaries, persistence-backed auth, runtime visibility, and secure data flow.

My work centers on:
- security-sensitive data flows
- compile-time invariants and typed workflows
- service boundaries and controlled data movement
- tooling that makes invalid states harder to represent

## Selected work

### [statum](https://github.com/eboody/statum)
Typestate framework for Rust. It enforces legal state transitions at compile time and supports rebuilding typed workflow state from persisted data.

### [eran.codes](https://github.com/eboody/eran.codes)
My personal site and lab. It is also a Rust codebase where I explore application structure, crate boundaries, runtime visibility, and UI experiments.

### [modum](https://github.com/eboody/modum)
Rust tooling for keeping module naming, import style, and public API paths consistent across a workspace.

### [nestum](https://github.com/eboody/nestum)
A Rust crate for making nested enums read more like nested paths, reducing friction around deeply structured state.

### [maud-extensions](https://github.com/eboody/maud-extensions)
Proc macros for Maud components with inline CSS, JS, slots, and font helpers.

## Systems work

In independent work, I built a multi-crate Rust healthcare integration platform with dedicated web, token, sync, auth, RPC, and core domain layers. The system handled EMR synchronization, encrypted PHI fields with AES-256-GCM, used Redis-backed token and lookup caching, and enforced explicit service boundaries around sensitive data access.

I have also built production automation and integration systems that replaced delayed manual workflows with realtime data movement, increased operator throughput substantially, and supported products used by major nonprofit organizations.

## What I care about

- boundaries that are visible in the code
- APIs that make illegal states difficult to express
- security properties enforced structurally, not socially
- tooling that improves correctness without making teams slower

## Links

- Website: [eran.codes](https://eran.codes)
- GitHub: [@eboody](https://github.com/eboody)
- LinkedIn: [Eran Boodnero](https://www.linkedin.com/in/eran-boodnero-602a994b/)

# Hi, I'm Eran

I'm a Rust-first software engineer building systems for healthcare and other sensitive-data work.

I like systems with sharp edges: healthcare integrations, encrypted PHI, sync jobs, auth and session flows, and state-heavy code that has to behave itself. If the work is sensitive, messy, or easy to get subtly wrong, that's usually where I'm having the most fun.

I also have a soft spot for automation. If a script can save me hours of repetitive work, I'm probably going to write it.

## Start here

- [Healthcare integration platform case study](./healthcare-integration-platform.md): sanitized writeup of EMR sync, encrypted PHI storage, token handling, and the public `eran.codes` demo that backs it up.
- [`eran.codes`](https://github.com/eboody/eran.codes): my current public Rust app showing encrypted storage, token handling, bounded sync, auth and sessions, and visible runtime behavior.
- [`statum`](https://github.com/eboody/statum): typestate framework for legal state transitions and rebuilding typed workflow state from persisted data.

## What I build

- healthcare integrations against the Elation EMR API
- encrypted storage for PHI fields
- Rust services with clear boundaries between external systems, app logic, and storage
- type-driven libraries focused on state, workflow, and API shape

## Production impact

- increased fundraiser acknowledgment throughput by roughly 12x per operator
- ran automation at 72 concurrent workers
- replaced a manual CSV process that lagged by 48 hours with realtime fundraiser creation and donation visibility
- supported products used by large national nonprofits

## More Rust projects

- [`modum`](https://github.com/eboody/modum): workspace lint tool for consistent module naming, import style, and public API paths.
- [`nestum`](https://github.com/eboody/nestum): proc macro for nested enum paths that keeps structured state readable without flattening it away.
- [`maud-extensions`](https://github.com/eboody/maud-extensions): proc macros for Maud components with inline CSS, JS, slots, and font helpers.

## Elsewhere

- Website: [eran.codes](https://eran.codes)
- GitHub: [@eboody](https://github.com/eboody)
- LinkedIn: [Eran Boodnero](https://www.linkedin.com/in/eran-boodnero-602a994b/)

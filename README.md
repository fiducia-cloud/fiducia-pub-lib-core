# Fiducia public library core

This repository is the public/external SDK boundary for Fiducia. It is kept
separate from `fiducia-lib-core` so public consumers can depend on a stable,
reviewable surface without inheriting internal implementation details.

## Contract-first scope

- Public types and wire contracts are sourced from `fiducia-interfaces`.
- Generated artifacts must be reproducible from their checked-in schemas and
  must not contain credentials, environment values, or host-specific paths.
- Language bindings are added only through the shared contract manifests; do
  not hand-edit generated output.
- Compatibility changes require an explicit versioning note and a migration
  path for downstream consumers.

The initial commit establishes the repository boundary. Public modules will be
introduced as their corresponding contracts are promoted from the internal
library with API and security review.

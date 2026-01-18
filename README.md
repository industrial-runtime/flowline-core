# Flowline Core

Flowline Core contains the **domain model, rules, and validation** for Flowline.
It is intentionally **pure**: no file system, no networking, no UI, no hardware access.

## Responsibilities
- Flow / step / transition domain model
- Deterministic state and transition rules
- Poka-Yoke enforcement rules (error prevention by design)
- Validation of flow definitions (structural and semantic)
- Ports (interfaces) for persistence, audit, time, and external interaction

## Non-Responsibilities
- No JSON parsing / serialization
- No database / file system access
- No networking / protocols
- No UI components
- No device drivers or hardware APIs

## Consumers
- `flowline-runtime`
- `flowline-tooling`
- `flowline-ui` (read-only domain usage)
- Integrations (through ports)

## Documentation
Architecture and decisions: see `flowline-docs` (especially `overview.md` and C4 diagrams).

## License
Apache License 2.0

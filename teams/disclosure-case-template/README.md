# Disclosure [Case Name]

> **Template.** Copy this whole directory to `teams/disclosure-<case-name>/`
> for each new case, then replace `[Case Name]` throughout.

A per-case workspace combining a **Chat Project** (review, audit, debugging)
and a **Cowork Project** (the actual execution).

## Chat Project — review & oversight

- [Pre-run review](./pre-run-review.md)
- [Audit](./audit.md)
- [One-off debugging](./one-off-debugging.md)

## Cowork Project — execution

- [execution/](./execution/) — the code that actually runs the disclosure

## Process

Run the stages in order, drawing each from the reusable library in
[`personal/workflows-and-architecture/playbooks/`](../../personal/workflows-and-architecture/playbooks/):

1. **Pre-run review** → go / no-go
2. **Execution** (in `execution/`)
3. **Audit**

…with **one-off debugging** as needed along the way. Register the case in the
[master tracker](../running-disclosures/active-disclosures-index.md).

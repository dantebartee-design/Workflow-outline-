# Workflows & Architecture *(Cowork Project)*

The reusable library. Every Teams disclosure case draws its process from the
playbook templates here, rather than reinventing it per case.

## Playbooks

The four reusable stages. Each is a **template** — copy into a case workspace
and fill in the case-specific detail.

- [Pre-run review](./playbooks/pre-run-review.md)
- [Run](./playbooks/run.md)
- [Audit](./playbooks/audit.md)
- [Debugging](./playbooks/debugging.md)

## How a case uses this library

```
teams/disclosure-<case>/        ← copies & instantiates these playbooks
        │
        └──► references ──► personal/workflows-and-architecture/playbooks/
                                    (the canonical, reusable source)
```

When a playbook improves on a real case, fold the lesson back into the template
here so the next case benefits.

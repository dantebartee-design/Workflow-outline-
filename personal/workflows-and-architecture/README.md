# Workflows & Architecture *(Cowork Project)*

The reusable library. Every Teams disclosure case draws its process from the
playbook templates here, rather than reinventing it per case.

## Playbooks

The reusable stages. Each is a **template** — copy into a case workspace and
fill in the case-specific detail.

- [Pre-run review](./playbooks/pre-run-review.md)
- [Run](./playbooks/run.md)
- [Audit](./playbooks/audit.md)
- [Debugging](./playbooks/debugging.md)
- [Debrief](./playbooks/debrief.md) — runs in Personal *after* the audit (see below)

## Where the messy code lives

Build-and-debug work is **not** here — it has its own standalone Personal Cowork
project: [`../build-and-debug/`](../build-and-debug/). Code is written and
debugged there, then **promoted** into the `playbooks/` library here once it's
proven. This project stays clean and reusable; the sandbox absorbs the mess.

## The learning loop

This library is not a one-way feed. It's a cycle:

```
   ┌─────────────────────── lessons (from the debrief) ───────────────────────┐
   │                                                                           │
   ▼                                                                           │
playbooks/  ──draws into──►  teams/disclosure-<case>/  ──pre-run → run → audit──►  Personal: debrief
 (library)                       (the case)                                        (feelings & learning)
```

- **Down/out:** a case copies & instantiates these playbooks.
- **Up/back:** after the case's audit (in Teams), the **debrief** happens back
  in Personal (`personal/disclosure-strategy/debriefs/`). Every lesson there is
  folded back into the templates here — *that edit is what closes the loop* and
  makes the next case start better.

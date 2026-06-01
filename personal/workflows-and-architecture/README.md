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

## Build & debug

- [build-and-debug/](./build-and-debug/) — the **messy sandbox** where
  disclosure code is actually written and debugged. Proven, generalized work is
  **promoted** from here into `playbooks/`. This is where the build-and-debug
  mess lives — deliberately, so cases and the clean library stay tidy.

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

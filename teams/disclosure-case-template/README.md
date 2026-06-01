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

- [execution/](./execution/) — **the Teams code** that actually runs the
  disclosure for this case. It *draws from* the Personal library
  (`personal/workflows-and-architecture/playbooks/`); it doesn't hold the only
  copy of anything reusable.

## Process

Steps are numbered to match the global [order of operations](../../README.md#order-of-operations--the-7-steps)
(steps 1–2 — building the reusable code — happen in Personal, before this).
Each stage draws from the reusable library in
[`personal/workflows-and-architecture/playbooks/`](../../personal/workflows-and-architecture/playbooks/):

3. **Pre-run review** → go / no-go
4. **Execution** *(code)* — run this case's code in `execution/`
5. **Audit** → *did it work?* — this is where the case ends, here in Teams.
6. **Debrief** → *what did I learn, how did it feel?* — this happens **back in
   Personal**, not here. Add `debrief-<case>.md` to
   [`personal/disclosure-strategy/debriefs/`](../../personal/disclosure-strategy/debriefs/).
7. **Fold lessons into the library** — edit the playbooks in Personal so the
   next case starts better.

…with **one-off debugging** as needed along the way. Register the case in the
[master tracker](../running-disclosures/active-disclosures-index.md).

> The audit stays in Teams; the debrief comes home to Personal. That handoff is
> what turns a finished case into a better next one.

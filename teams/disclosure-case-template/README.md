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
3. **Audit** → *did it work?* — this is where the case ends, here in Teams.
4. **Debrief** → *what did I learn, how did it feel?* — this happens **back in
   Personal**, not here. Add `debrief-<case>.md` to
   [`personal/disclosure-strategy/debriefs/`](../../personal/disclosure-strategy/debriefs/),
   and fold its lessons into the playbook library.

…with **one-off debugging** as needed along the way. Register the case in the
[master tracker](../running-disclosures/active-disclosures-index.md).

> The audit stays in Teams; the debrief comes home to Personal. That handoff is
> what turns a finished case into a better next one.

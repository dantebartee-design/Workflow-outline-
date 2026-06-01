# Workflow Outline

![Workflow structure](docs/structure.png)

A repository scaffold mirroring how Disclosure work is organized across
**Personal** and **Teams** spaces, using a mix of *Chat Projects* (thinking,
tracking, review) and *Cowork Projects* (code and execution).

This repo is the source of truth for **structure and reusable playbook
templates**. Individual chats live in the product; the files here capture the
durable artifacts — indexes, status, vision notes, and the reusable playbooks
that any disclosure run draws from.

## Top-level map

```
PERSONAL
├── Disclosure Strategy        (Chat Project)   → personal/disclosure-strategy/
│     └── debriefs/            post-case "feelings & learning" → personal/disclosure-strategy/debriefs/
├── Personal Explorations      (Chat Project)   → personal/personal-explorations/
├── Workflows & Architecture   (Cowork Project) → personal/workflows-and-architecture/
│     └── playbooks/           the reusable library (incl. debrief)
└── Build & Debug              (Cowork Project) → personal/build-and-debug/
      └── messy code sandbox → promoted into Workflows & Architecture

TEAMS
├── Running Disclosures        (Chat Project)   → teams/running-disclosures/        (master tracker)
├── Disclosure [Case Name]     (Chat Project)   → teams/disclosure-case-template/   (per-case review/audit/debug)
└── Disclosure [Case Name]     (Cowork Project) → teams/disclosure-case-template/execution/  (the actual run)
```

## Project types

| Type | Purpose | Lives where |
|------|---------|-------------|
| **Chat Project** | Thinking, vision, review, audit, tracking | `*/README.md` + topic notes |
| **Cowork Project** | Code, playbooks, and execution of a run | `workflows-and-architecture/`, `*/execution/` |

## How the pieces connect

- **Personal → Workflows & Architecture** holds the *reusable* playbooks
  (pre-run review, run, audit, debugging, debrief) — the clean library.
- **Personal → Build & Debug** is a separate Cowork project: the messy sandbox
  where disclosure code is written and debugged, then **promoted** into the
  Workflows & Architecture library once proven.
- **Teams → Running Disclosures** is the master tracker: one index, one status
  view across every active and planned case.
- **Teams → Disclosure [Case Name]** is a per-case workspace. Copy
  `teams/disclosure-case-template/` for each new case; its playbooks point back
  to the reusable library in Personal.

### The learning loop

This is a **cycle**, not a one-way pipeline:

```
library  ──draws into──►  case (pre-run → execution → audit, in Teams)
   ▲                                      │
   │                                      ▼
   └──── lessons ◄──── debrief (back in Personal: feelings & learning)
```

The **audit stays in Teams** (*did it work?*). The **debrief comes home to
Personal** (*what did I learn, how did it feel?*). Each debrief's lessons are
folded back into the library — that return edit is what makes the next case
start better.

## Starting a new disclosure

1. Copy `teams/disclosure-case-template/` to `teams/disclosure-<case-name>/`.
2. Add the case to `teams/running-disclosures/active-disclosures-index.md`.
3. Work the playbooks in order: **pre-run review → execution → audit**, with
   **one-off debugging** as needed.
4. After the audit, **debrief back in Personal**: add
   `personal/disclosure-strategy/debriefs/debrief-<case>.md`, then fold its
   lessons into `personal/workflows-and-architecture/playbooks/`.

See each directory's `README.md` for detail.

# Claude Workflow System — Complete Reference

> A single place to understand how work flows from **idea → build → run → learn → automate**.
> Built to be readable on a phone, printable on paper, and clear enough to reference without scrolling through a long chat.

---

## Table of Contents

1. [Workflow Overview](#1-workflow-overview)
2. [Project Structure](#2-project-structure)
3. [The Action Plan — In Order](#3-the-action-plan--in-order)
4. [Folder Structure](#4-folder-structure)
5. [Key Concepts](#5-key-concepts)
6. [Conversation Map](#6-conversation-map)
7. [Long-term Vision](#7-long-term-vision)

---

## 1. Workflow Overview

**⭐ North Star — Step 0: Vision**
The North Star sits above everything. It informs every step. Before you build, run, or automate anything, the Vision tells you *why* and *toward what*. Every other step bends back to serve it.

Then seven steps, in order:

| Step | Name | Where it lives | What happens |
|------|------|----------------|--------------|
| **0** | ⭐ **Vision** | Above everything | The North Star that informs every step |
| **1** | **Build & Debug** | Personal **Cowork** | Messy code lives here. You experiment, break things, iterate |
| **2** | **Promote to Library** | → Workflows & Architecture | When proven, code moves into the library |
| **3** | **Pre-run Review** | Teams **Chat** | Quality gate. Check before you run for real |
| **4** | **Execution** | Teams **Cowork** | The actual run |
| **5** | **Audit** | Teams **Chat** | Nuts and bolts of what actually happened |
| **6** | **Debrief** | Personal **Chat** | Feelings and learning — home after the audit |
| **7** | **Fold Lessons Back** | → Vision + Library | Update the Vision and the Library based on what you learned |

**The loop:** Step 7 feeds back into Step 0 and Step 2. The system gets smarter every cycle.

```
        ⭐ STEP 0: VISION (North Star)
                  │  informs everything
                  ▼
   ┌──────────────────────────────────────┐
   │  1. Build & Debug      (Personal Cowork)
   │  2. Promote to Library (→ Library)
   │  3. Pre-run Review     (Teams Chat)
   │  4. Execution          (Teams Cowork)
   │  5. Audit              (Teams Chat)
   │  6. Debrief            (Personal Chat)
   │  7. Fold Lessons Back  (→ Vision + Library)
   └──────────────────────────────────────┘
                  │
                  └──── feeds back to Step 0 & Step 2
```

---

## 2. Project Structure

Two worlds: **Personal** and **Teams**. Within each, two kinds of project:

- **Chat Projects** → conversation, thinking, feedback.
- **Cowork Projects** → executable work and code.

### 👤 Personal

| Project | Type | Purpose |
|---------|------|---------|
| **Disclosure Strategy** | Chat | High-level strategy and thinking |
| **Personal Explorations** | Chat | Open-ended exploration, feelings, learning |
| **Workflows & Architecture** | Cowork | **The library** — proven code, playbooks, diagrams |

### 👥 Teams

| Project | Type | Purpose |
|---------|------|---------|
| **Running Disclosures** | Chat | **Master tracker** — status across all cases |
| **Disclosure [Case Name]** | Chat | Pre-run review, audit, debugging |
| **Disclosure [Case Name]** | Cowork | Execution — the actual run |

---

## 3. The Action Plan — In Order

### Phase 1 — Cleanup & Foundation

- [ ] **Create "Claude Cleanup and Reorganization" project**
  - Audit existing files
  - Decide: keep / move / delete
  - Set up folder structure
- [ ] **Create "Workflows and Architecture" project** (the library)
  - Pin this conversation summary
  - Pin the workflow diagram
  - Create the **Value Timeline** document

### Phase 2 — Setup Before Next Disclosure

- [ ] Set up folder structure (Personal **and** Teams projects)
- [ ] Create **"Lawyer Ideas and Requests"** project (Teams Chat)
- [ ] Create **Lawyer Playbook Template** (one-page, simple)

### Phase 3 — Execution: Disclosure Two & Beyond

- [ ] **Run Disclosure Two using the new workflow**
  - Follow North Star + seven steps
  - Document as you go
  - Debrief in Personal
  - Extract the lawyer playbook
- [ ] After Disclosure Two → **update Value Timeline with real data**

### Phase 4 — Optimization: After Two-to-Three Disclosures

- [ ] **Design Agent / Automation Strategy** (assess what can be automated)
- [ ] **Build & Test First Agent** (lives in Workflows & Architecture, executes the proven playbook)
- [ ] **Hand Off to Lawyer** (agent runs autonomously; you review and approve)

---

## 4. Folder Structure

```
CLAUDE WORKSPACE
│
├── 👤 PERSONAL
│   │
│   ├── 💬 Disclosure Strategy            [Chat Project]
│   │      └─ strategy & thinking
│   │
│   ├── 💬 Personal Explorations          [Chat Project]
│   │      └─ exploration, feelings, learning
│   │           ▲
│   │           │  (Step 6: Debrief lands here)
│   │
│   └── 🛠️ Workflows & Architecture       [Cowork Project] ← THE LIBRARY
│          ├─ pinned: workflow diagram
│          ├─ pinned: conversation summary
│          ├─ Value Timeline document
│          ├─ proven playbooks
│          └─ agents (later)
│
└── 👥 TEAMS
    │
    ├── 💬 Running Disclosures             [Chat Project] ← MASTER TRACKER
    │      └─ status across all cases
    │
    ├── 💬 Disclosure [Case Name]          [Chat Project]
    │      └─ pre-run review · audit · debugging
    │
    └── 🛠️ Disclosure [Case Name]          [Cowork Project]
           └─ execution — the actual run
```

### How they connect (conversation flow)

```
  Build (Personal Cowork)
        │  proven code
        ▼
  Workflows & Architecture (Library) ──────┐
        │  pull playbook                    │ folds lessons back (Step 7)
        ▼                                   │
  Pre-run Review (Teams Chat) ─► Execution (Teams Cowork)
        │                                   │
        ▼                                   ▼
  Audit (Teams Chat) ──────────────► Debrief (Personal Chat)
        │                                   │
        └──────────► Running Disclosures ◄──┘
                     (Master Tracker watches it all)
```

- **Vision** sits above and informs every box.
- **Execution** happens in Teams Cowork, reviewed before (Pre-run, Teams Chat) and after (Audit, Teams Chat).
- **Debrief** is the trip home — Personal Chat.
- **Lessons** flow back up into the Library and the Vision.

---

## 5. Key Concepts

### Cowork vs. Chat

| | **Cowork** | **Chat** |
|---|------------|----------|
| **What** | Executable, actionable work | Conversation, thinking, feedback |
| **Contains** | Code or structure you'll reuse | Linear discussion |
| **Reused?** | Yes — pulled into other work | No — doesn't need pulling into another project |

### Projects vs. Random Chats

| | **Projects** | **Random Chats** |
|---|--------------|------------------|
| **Shape** | Grouped, related conversations | One-off, standalone |
| **Theme** | One theme you reference repeatedly | No ongoing theme |
| **Use when** | You'll come back to it | You won't |

### The Lawyer Playbook Separation

> Keep the clean front-stage separate from the messy back-stage.

| **What the lawyer sees** | **What you build internally** |
|--------------------------|-------------------------------|
| Clean deliverable | All the iterations |
| Simple playbook | The debates |
| Status updates | The cleanup |
| | The learning |

The lawyer gets the polished result. You keep the workshop.

### The Value Timeline

Three timelines, side by side — the case for the system.

| | **Timeline 1: No System** | **Timeline 2: With System** | **Timeline 3: With Automation** |
|---|---------------------------|------------------------------|----------------------------------|
| **What** | What they did before | The system in use | Agents running it |
| **Disclosure 1** | 12–15 hrs | 12 hrs (building) | — |
| **Disclosure 2** | 12–15 hrs | 6 hrs (refining) | — |
| **Disclosure 3** | 12–15 hrs | 4 hrs (executing) | — |
| **Disclosure 4+** | 12–15 hrs | — | **30 min to trigger** (runs autonomously) |

```
Time per disclosure
15h │ ███████████████  No system (flat, forever)
12h │ ███████████      System: build
 6h │ ██████           System: refine
 4h │ ████             System: execute
0.5h│ ▌                Automation: trigger
    └────────────────────────────────────
     D1   D2   D3   D4+
```

The line bends down. Without the system, it never does.

---

## 6. Conversation Map

Which conversations to have, when, and with whom.

### 🟢 Start Next

| Conversation opener | Where |
|---------------------|-------|
| "I need to clean up my Claude files" | Cleanup project |
| "Help me document the disclosure workflow" | Workflows & Architecture |
| "Help me create a folder structure template" | Claude Code |

### 🔵 Start After Cleanup

| Conversation opener | Where |
|---------------------|-------|
| "Help me organize the lawyer's requests" | Lawyer Ideas and Requests |
| "Help me create a playbook template" | For the lawyer |

### 🟣 Start With Disclosure Two

| Conversation opener | Where |
|---------------------|-------|
| "Let's run disclosure two using the new workflow" | Actual work |
| "Help me debrief" | Personal |
| "Help me package the value" | For the lawyer |

### 🟠 Start After Two-to-Three Disclosures

| Conversation opener | Where |
|---------------------|-------|
| "Help me design automation" | Agents & API strategy |
| "Help me build an agent" | Actual agent building |

---

## 7. Long-term Vision

**The automation path** — three phases. You don't skip ahead.

### Phase 1 — Do it manually
You're doing disclosures by hand. Learning the process. Documenting it. Debriefing.

### Phase 2 — Build the playbook
You've done it a few times. You have a solid, proven playbook.

### Phase 3 — Teach an agent
Using the **Agent SDK** and your **API key**, you teach an agent to follow that playbook.

> **The agent doesn't invent the process — it executes the one you've proven works.**

**Two rules that keep this honest:**

1. Agents live in **Workflows & Architecture** — but **only after** you've proven the manual process.
2. **The agent is the automation version of a playbook that already exists.** No playbook, no agent.

```
Phase 1: Manual      → learn + document + debrief
Phase 2: Playbook    → proven, repeatable
Phase 3: Agent       → executes the proven playbook (Agent SDK + API key)

        Manual proof ──► Playbook ──► Agent
        (never the other way around)
```

---

*End of reference. Update this document in **Workflows & Architecture** whenever Step 7 folds new lessons back in.*

# Build & Debug *(Cowork Project)*

> **Step 1** of the [7-step order](../../README.md#order-of-operations--the-7-steps),
> and the first of the two Personal code locations. This is where code is born.

A standalone Personal Cowork project — the **messy workspace** where disclosure
code actually gets built and debugged before it's clean enough to be reusable.

This is its own project (a sibling of *Workflows & Architecture*), on purpose:
experimentation, spikes, and half-working code live here, separate from both the
polished library and any Teams case. It's the answer to "where does the messy
build-and-debug work live?" — **here**.

## The promotion path

```
personal/build-and-debug/              (messy: spikes, experiments, throwaway scripts)
        │  once it's proven and generalized
        ▼
personal/workflows-and-architecture/   (clean: the reusable library every case draws from)
        playbooks/
```

Build freely here. When something works and is worth reusing, **promote** it:
generalize it and move/encode it into
[`../workflows-and-architecture/playbooks/`](../workflows-and-architecture/playbooks/).
Don't let a Teams case depend on code that still lives in this sandbox.

## Relationship to the rest of the system

- **Build & Debug** (this project) → messy code is born here.
- **Workflows & Architecture** → proven code is promoted into the clean library.
- **Teams cases** → only ever draw from the clean library, never from here.

# Build & Debug *(sandbox)*

The **messy workspace** — where disclosure code actually gets built and
debugged before it's clean enough to be reusable.

This sits inside the Personal *Workflows & Architecture* Cowork project on
purpose: experimentation and half-working code live here, not in a Teams case
and not in the polished library. It's the answer to "where does the messy
build-and-debug work live?" — **here**.

## The promotion path

```
build-and-debug/   (messy: spikes, experiments, throwaway scripts)
        │  once it's proven and generalized
        ▼
playbooks/         (clean: the reusable library every case draws from)
```

Build freely here. When something works and is worth reusing, **promote** it:
generalize it and move/encode it into `../playbooks/`. Don't let a Teams case
depend on code that still lives in this sandbox.

> If this sandbox ever grows big enough to deserve its own Personal Cowork
> project, split it out — but for now it's folded into the library project.

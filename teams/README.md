# Teams

Shared workspace for running disclosures with a team.

- **[Running Disclosures](./running-disclosures/)** *(Chat Project — Master
  Tracker)* — the single index and status view across all cases.
- **[Disclosure Case Template](./disclosure-case-template/)** — copy this for
  each new case. Contains the per-case Chat workspace (pre-run review, audit,
  debugging) and the `execution/` Cowork project (the actual run).

## Per-case convention

For a new case named e.g. `acme`:

```
cp -r teams/disclosure-case-template teams/disclosure-acme
```

Then register it in [running-disclosures/active-disclosures-index.md](./running-disclosures/active-disclosures-index.md).

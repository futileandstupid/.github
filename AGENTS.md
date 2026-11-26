# `futileandstupid/.github` — Account Community Health Instructions

## Role
Provides default account-wide GitHub community health documents inherited by all repositories under `futileandstupid` unless overridden locally:
- [`SECURITY.md`](SECURITY.md) — Coordinated vulnerability disclosure policy (GitHub Private Vulnerability Reporting).
- [`SUPPORT.md`](SUPPORT.md) — Issue routing and verification expectations.
- [`CONTRIBUTING.md`](CONTRIBUTING.md) — **Permit-and-Contract Engineering (`PCE`)** and **JBC Edition 1.3** contribution standards (no Agile user stories or unverified prose checklists).

## Governance & Protected Branch Ruleset
- `main` enforces ruleset `main-protection` (`require_pr = true`, `require_linear_history = true`, `bypass_actors = []`).
- Never push directly to `main`; create a `chore/*` or `docs/*` branch, open a pull request (`gh pr create`), and squash-merge (`gh pr merge --squash --delete-branch`).
- Account-wide repository settings and rulesets across all `futileandstupid` repositories are reconciled declaratively by sibling private repository `futileandstupid/steward` (`fleet.toml`).

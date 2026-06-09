---
"@chbrain/khai-plays-kleist": patch
---

Record management order 260609_1: guard `main`. The house runs on lane PRs but
`main` is not yet branch-protected, so the gate checks only advise. The order
directs the human to require pull requests and the `test` / `khai-guard` /
`branch-scope` / `consistency` checks, and to forbid force-pushes and deletion —
a khai-stage handoff the agent's tools cannot perform.

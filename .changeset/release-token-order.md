---
"@chbrain/khai-plays-kleist": patch
---

Record management order 260609_2: set `RELEASE_TOKEN`. The changeset wiring
matches Buechner, but the release workflow fails for want of the
`RELEASE_TOKEN` secret, so no Version Packages PR opens and the house publishes
nothing. The order directs the human to add the PAT secret — a khai-stage
handoff the agent's tools cannot perform.

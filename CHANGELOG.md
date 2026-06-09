# @chbrain/khai-plays-kleist

## 0.1.0

### Minor Changes

- 50346b3: Stage Heinrich von Kleist's comedic masterpiece _Der zerbrochne Krug_ (The Broken Jug) as a complete systemic model, establishing the play definition, 6 personas, 5 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.

### Patch Changes

- eab0df7: Add play-level `README.md` and `REFERENCES.md` for _Der zerbrochne Krug_.
- 138b3aa: Record resolution of management orders 260609_2 and 260609_3. Marks order 260609_2 (setting the RELEASE_TOKEN secret) as closed now that the release workflow has run and opened the Version Packages PR, and marks order 260609_3 (staging Der zerbrochne Krug) as closed now that the complete flat play system and documentation are merged to main.
- d347338: Record management order 260609_1: guard `main`. The house runs on lane PRs but
  `main` is not yet branch-protected, so the gate checks only advise. The order
  directs the human to require pull requests and the `test` / `khai-guard` /
  `branch-scope` / `consistency` checks, and to forbid force-pushes and deletion —
  a khai-stage handoff the agent's tools cannot perform.
- 74968e7: Harden the CI/audit workflows against GitHub Actions expression injection. Untrusted
  contexts (PR branch names via `github.head_ref` / `steps.*.outputs.*_ref`, the PR
  number, and the diff-derived audit ids) are no longer interpolated directly into
  `run:` shell or `github-script` bodies; they pass through `env:` and are referenced
  as `"$VAR"` / `process.env.*`. Clears the code-scanning expression-injection
  findings; no behavioral change to the gates. Mirrors the hardened khai-stage blueprint.
- 0ee5e94: Record management order 260609_2: set `RELEASE_TOKEN`. The changeset wiring
  matches Buechner, but the release workflow fails for want of the
  `RELEASE_TOKEN` secret, so no Version Packages PR opens and the house publishes
  nothing. The order directs the human to add the PAT secret — a khai-stage
  handoff the agent's tools cannot perform.
- daf930f: Update `REFERENCES.md` with the complete Heinrich von Kleist works catalog, German staging language policy, and staging status.
- e8f455a: Upgrade `@chbrain/khai-arch` and `@chbrain/khai-tests` packages to their latest versions, enforce LF line endings with `.gitattributes` to resolve Windows build failures, and add `.gitattributes` to the shared paths list in `khai-guard.config.json`.

# @chbrain/khai-plays-kleist

## 0.2.0

### Minor Changes

- 0bfd5f0: Stage Heinrich von Kleist's Lustspiel _Amphitryon_ (1807) as a complete systemic model, establishing the play definition, 6 personas, 6 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- 75611e0: Stage Heinrich von Kleist's novella _Das Erdbeben in Chili_ (1807) as a complete systemic model, establishing the play definition, 6 personas, 6 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- 10fed78: Stage Heinrich von Kleist's tragedy _Die Familie Schroffenstein_ (The Schroffenstein Family) as a complete systemic model, establishing the play definition, 6 personas, 6 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- 88afe7d: Stage Heinrich von Kleist's novella _Die Marquise von O..._ (1808) as a complete systemic model, establishing the play definition, 6 personas, 6 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- 86ce2b7: Stage Heinrich von Kleist's novella _Michael Kohlhaas_ (1810) as a complete systemic model, establishing the play definition, 6 personas, 6 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- c1f9e5d: Stage Heinrich von Kleist's tragedy _Penthesilea_ as a complete systemic model, establishing the play definition, 6 personas, 6 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- 07bce75: Stage Heinrich von Kleist's celebrated drama _Prinz Friedrich von Homburg_ (The Prince of Homburg) as a complete systemic model, establishing the play definition, 6 personas, 6 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- 70c7af5: Stage Heinrich von Kleist's tragedy fragment _Robert Guiskard_ (1808) as a complete systemic model, establishing the play definition, 6 personas, 6 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.

### Patch Changes

- 9f5cdad: Bump the `@chbrain/*` dev dependencies to the latest published canon:
  `khai-arch` 0.1.14, `khai-review` 0.1.3, `khai-tests` 0.1.17. The house
  conforms against the updated canon (tests green).
- 3b0a035: Rename the CI conformance job from `test` to `khai-tests`, the tool it runs,
  matching the `khai-guard` job's naming and the khai-stage blueprint. Branch
  protection must require the `khai-tests` check instead of `test` once this
  lands.
- 33566bf: Record resolution of management order 260610_1. Marks the order for staging Prinz Friedrich von Homburg as closed and all its targets as completed.
- 33997b5: Re-declare play content license under CC-BY-NC-SA-4.0 for all staged plays: Der zerbrochne Krug, Prinz Friedrich von Homburg, Penthesilea, and Die Familie Schroffenstein.
- 26735c6: Update root-level `REFERENCES.md` staging status to mark _Amphitryon_ as staged and add _Robert Guiskard_ as planned.
- 47bb52a: Update root-level `REFERENCES.md` staging status to mark _Das Erdbeben in Chili_ as staged and add _Die Verlobung in St. Domingo_ as planned.
- 50d6fdd: Update root-level `REFERENCES.md` staging status to mark _Robert Guiskard_ as staged and add _Die Marquise von O..._ as planned.
- 8dfc416: Update root-level `REFERENCES.md` staging status to mark _Michael Kohlhaas_ as staged and add _Amphitryon_ as planned.
- 5791bfa: Update root-level `REFERENCES.md` staging status to mark _Die Marquise von O..._ as staged and add _Das Erdbeben in Chili_ as planned.
- d89a71b: Update root-level `REFERENCES.md` with the staging status of the completed Kleist plays: _Prinz Friedrich von Homburg_, _Penthesilea_, and _Die Familie Schroffenstein_.

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

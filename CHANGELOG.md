# @chbrain/khai-plays-kleist

## 0.22.6

### Patch Changes

- 1aac1be: Add a pitch (the tonal key: tenor, undertow, nerve, echo) to every Kleist play, in German in Kleist's register and wired into each play's Company. 24 pitches across 22 plays.

## 0.22.5

### Patch Changes

- 35e501c: Converge kleist management onto the shared blueprint core (Order 0c). The voice layer
  and the chain-owned core (positions, shared Choregos personas, plan_stage_the_score)
  now match the blueprint verbatim; cast the house Director (Heinrich Laube) as overlay.
  Touring deferred (Kleist has none yet). The convergence gate reports 0 findings; house conformance passes.
- e80782f: Sync the Director position to the current blueprint: the cast named as the
  producer (the separation of two stances), and "tune the pitch" added to the
  redirect idioms. Brings the house in line with the chain canon (khai #505/#506).
- e7dd228: Re-converge the Director seat to the control loop: position_director and
  plan_stage_the_score match the rewritten blueprint core (the Director runs a
  living production and captures a run, not a teller).

## 0.22.4

### Patch Changes

- 4a7bcd0: plays: English shelf loglines. Add an English `description:` to every play's
  frontmatter and regenerate registry.json, so the registry (the English-facing
  index the website overview reads) carries English loglines while the German
  `## Arc` stays the book's synopsis. Also bumps `@chbrain/khai-tests` to 0.1.21,
  which reads the frontmatter `description`. 22 plays.

## 0.22.3

### Patch Changes

- c4de84f: deps: bump `@chbrain/khai-tests` to 0.1.20 (lockfile), which adds the `titleLeakAudit` reviewer-assist. Conformance stays green; the assist surfaces source-language-in-`title:` candidates as audit notes only.

## 0.22.2

### Patch Changes

- 8e7397c: data: remove the lone en-dash from the Berliner Abendblätter README year range (`1810–1811` -> `1810 to 1811`), per the global no-dash rule. The only literal dash in the Kleist play sources.
- 0d3c16f: governance: rebuild the house `voice` so it no longer endorses the dash, which contradicts the global no-dash rule. Kleist's essential character is kept (periodic, deeply subordinated sentences where certainty breaks) but the mechanism now rests on the period, the colon, and subordination instead of the dash. No play prose is changed.

## 0.22.1

### Patch Changes

- 1e6196b: data: translate element and play `title` frontmatter into English display names, keeping the German original in `declared`. Kleist shipped German in both fields (`title: "Der Identitätsdiebstahl"`), unlike the sibling Büchner house which already separates an English `title` from a German `declared`. The `title` is what the website renders on the shelf and the call board, so it now reads English (`Identity Theft`, `Thebes`, `The Broken Jug`) while `declared` keeps the German. Proper names (Penthesilea, Michael Kohlhaas, Käthchen) are unchanged; filenames (ids), `#el-<id>` links, and prose are untouched.

## 0.23.0

### Minor Changes

- 118d1ef: Stage Heinrich von Kleist's daily journal _Berliner Abendblätter_ (1810-1811) as a complete systemic model, establishing the play definition, 3 personas, 3 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- eaefe39: Stage Heinrich von Kleist's novella _Das Bettelweib von Locarno_ (1810) as a complete systemic model, establishing the play definition, 6 personas, 6 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- fb12464: Stage Heinrich von Kleist's historical knightly play _Das Käthchen von Heilbronn_ (1810) as a complete systemic model, establishing the play definition, 6 personas, 6 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- aaf1165: Stage Heinrich von Kleist's novella _Der Findling_ (1811) as a complete systemic model, establishing the play definition, 6 personas, 6 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- 118d1ef: Stage Heinrich von Kleist's novella _Der Zweikampf_ (1811) as a complete systemic model, establishing the play definition, 3 personas, 3 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- b1c4345: Stage Heinrich von Kleist's legend _Die heilige Cäcilie oder die Gewalt der Musik_ (1810) as a complete systemic model, establishing the play definition, 6 personas, 6 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- d980806: Stage Heinrich von Kleist's historical drama _Die Hermannsschlacht_ (1808) as a complete systemic model, establishing the play definition, 6 personas, 6 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- ba7c501: Stage Heinrich von Kleist's biographical crisis play _The Kant Crisis_ (1801) as a complete systemic model, establishing the play definition, 3 personas, 2 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- ba7c501: Stage Heinrich von Kleist's biographical crisis play _Recovery of the Nachlass_ (1821) as a complete systemic model, establishing the play definition, 3 personas, 3 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- 225c98c: Stage Heinrich von Kleist's essay _Über die allmähliche Verfertigung der Gedanken beim Reden_ (1878) as a complete systemic model, establishing the play definition, 6 personas, 6 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- ba7c501: Stage Heinrich von Kleist's biographical crisis play _The Wannsee Pact_ (1811) as a complete systemic model, establishing the play definition, 3 personas, 3 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.

### Patch Changes

- d475610: Re-scope the management house to English. The management instances (the production apparatus: Kleist, the Choregos, the Playwright, the Theatre Manager) are English content, not in-world German staging, so each declares `language: english` in frontmatter and carries no German `declared`.
- ef7d05d: Ship the play registry in the published package by adding `registry.json` to the `files` array in `package.json`.
- 5218663: Update root-level `REFERENCES.md` staging status to mark _Der Findling_ as staged and add _Die heilige Cäcilie oder die Gewalt der Musik_ as planned.
- ef16368: Update root-level `REFERENCES.md` staging status to mark _Die Hermannsschlacht_ as staged and add _Der Findling_ as planned.
- e1aa1c6: Update root-level `REFERENCES.md` staging status to mark _Das Käthchen von Heilbronn_ as staged and add _Die Hermannsschlacht_ as planned.
- cf0c25e: Update root-level `REFERENCES.md` staging status to mark _Die heilige Cäcilie oder die Gewalt der Musik_ and _Das Bettelweib von Locarno_ as staged, and add _Über die allmähliche Verfertigung der Gedanken beim Reden_ as planned.
- f8af910: Update root-level `REFERENCES.md` staging status to mark _Über das Marionettentheater_ as staged.
- 98fce45: Update root-level `REFERENCES.md` staging status to mark _Über die allmähliche Verfertigung der Gedanken beim Reden_ as staged.

## 0.12.0

### Minor Changes

- 3252c88: Stage Heinrich von Kleist's novella _Die Verlobung in St. Domingo_ (1811) as a complete systemic model, establishing the play definition, 6 personas, 6 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.
- 5227fa2: Stage Heinrich von Kleist's philosophical essay _Über das Marionettentheater_ (1810) as a complete systemic model, establishing the play definition, 6 personas, 6 positions, 1 place, 1 piece, 1 plot, 1 plan, and 1 process.

### Patch Changes

- c86d7ef: Sync @chbrain/khai-tests to ^0.1.19 and let the version script heal registry.json (`changeset version && khai-tests registry build`); cast each plot's company inline so the casting gate holds.
- 07c39be: Update root-level `REFERENCES.md` staging status to mark _Die Verlobung in St. Domingo_ as staged and add _Über das Marionettentheater_ as planned.

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

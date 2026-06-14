---
"@chbrain/khai-plays-kleist": patch
---

data: translate element and play `title` frontmatter into English display names, keeping the German original in `declared`. Kleist shipped German in both fields (`title: "Der Identitätsdiebstahl"`), unlike the sibling Büchner house which already separates an English `title` from a German `declared`. The `title` is what the website renders on the shelf and the call board, so it now reads English (`Identity Theft`, `Thebes`, `The Broken Jug`) while `declared` keeps the German. Proper names (Penthesilea, Michael Kohlhaas, Käthchen) are unchanged; filenames (ids), `#el-<id>` links, and prose are untouched.

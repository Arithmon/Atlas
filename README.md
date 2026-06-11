# The Arithmon Atlas

An annotated map of work adjacent to the [Arithmon program](https://github.com/arithmon):
from information geometry to structural realism, from G2 constructions to
exact mass relations. Not a list of links. A living document that grows with
every reading and every contact.

See [INDEX.md](INDEX.md) for the current map, by relation and by domain.

## What an entry is

One file per work in [`entries/`](entries/), three content fields, nothing else:

- **Claim.** What the work asserts, stated so its author would sign it.
- **Relation.** One of `convergent`, `divergent`, `orthogonal`, then one
  clause of justification. Intensity and hybrids live in the prose; the
  frontmatter value stays a strict one-of-three so the atlas is filterable.
- **Δ.** The precise difference. The strongest deltas cut both ways: what
  Arithmon does that the neighbor does not, and what the neighbor has that
  Arithmon lacks.

## Frontmatter schema

```yaml
title: Human-readable work title
authors: Names, semicolon-separated
domain: mathematics | physics | philosophy | methods
relation: convergent | divergent | orthogonal
status: read | skimmed | to-read
ref: One canonical citation (journal, arXiv, book)
added: YYYY-MM-DD
```

## Rules

1. **Admission.** An entry earns its place if and only if its delta fits in
   one precise sentence. If the delta cannot be written, the work is either
   not adjacent enough or not yet understood: it goes to the to-read shelf,
   not into the atlas.
2. **Courtesy.** Every entry is written so that its author would sign the
   Claim and recognize the Δ as fair. The delta describes; it never grades.
   Divergent entries are first-contact material, not polemics.
3. **No silent edits.** A change of `relation` is a finding; it gets a dated
   note in the entry, not a silent overwrite.

## Contributing

Entries can be proposed by pull request. The schema above is checked by
`scripts/build_index.py`, and the organization prose gate runs in CI. The
admission and courtesy rules apply to contributions as they do to the
maintainer.

## Index

`INDEX.md` is generated from the frontmatter: `python scripts/build_index.py`.
Do not edit it by hand.

---

<sub>GIFT is the founding framework of the Arithmon program.
Program: [arithmon.com](https://arithmon.com) ·
[github.com/arithmon](https://github.com/arithmon)</sub>

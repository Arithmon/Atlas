# Contributing to the Atlas

The Atlas maps work adjacent to the Arithmon program. The unit of contribution
is one entry for one work, with a precise relation and a precise delta. A good
entry is one its own author would sign.

Org-wide rules (what helps, what does not, house style) are in the
[organization CONTRIBUTING](https://github.com/arithmon/.github/blob/main/CONTRIBUTING.md).
The entry format is specified in the [README](README.md); this file is the
how-to.

## Propose an entry

1. Pick the work. It can be convergent (it points the same way), divergent (it
   contradicts something Arithmon claims), or orthogonal (it is nearby but
   independent). All three are wanted. Divergent entries are especially wanted:
   an atlas of only friendly neighbours is a brochure, not a map.
2. Add one file under [`entries/`](entries/), following the frontmatter schema
   in the README. The `relation` field is a strict one-of-three
   (`convergent | divergent | orthogonal`) so the map stays filterable;
   intensity and nuance go in the prose.
3. Write the three fields, nothing else:
   - **Claim.** What the work asserts, stated so its author would agree.
   - **Relation.** The one-of-three value, then one clause of justification.
   - **Δ.** The precise difference, cutting both ways: what Arithmon does that
     this work does not, and what this work has that Arithmon lacks. An entry
     whose Δ only flatters Arithmon will be sent back.
4. Do not edit `INDEX.md` by hand. It is generated:
   `python scripts/build_index.py`.

## What makes an entry good

- It reads the source, not the abstract. Mischaracterising a neighbour is worse
  than omitting it.
- Its Δ is specific enough to be wrong. "Related in spirit" is not a delta.
- It is honest about divergence. If a respected result cuts against Arithmon,
  that is exactly what the Atlas is for.

## What does not belong

- Promotional comparisons ("unlike X, Arithmon..."). State the delta, let the
  reader rank.
- Link lists with no claim, relation, or delta.
- Entries that force a work into the Arithmon taxonomy. Map the neighbour by its
  own contours.

---

Siblings: [Program](https://github.com/arithmon/program) ·
[Sieve](https://github.com/arithmon/sieve) ·
[Lean](https://github.com/arithmon/lean)

<sub>GIFT is the founding framework of the Arithmon program.
Program: [arithmon.com](https://arithmon.com) ·
[github.com/arithmon](https://github.com/arithmon)</sub>

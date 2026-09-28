# Bowron's ED-space conjecture

A short proof of the ED-space conjecture stated in the Closing Remarks of Mark Bowron's paper:

> Mark Bowron, *Boundary-border extensions of the Kuratowski monoid*,  
> **Topology and its Applications** 341 (2024), 108703.  
> DOI: 10.1016/j.topol.2023.108703  
> arXiv:2210.10928

Bowron uses the operators `b` for closure, `i` for interior, and `f` for boundary. The conjecture asks whether every ED space in his classification contains a nonempty subset `A` such that

```
bA = ifA.
```

The proof is contained in [`ed_space_conjecture.tex`](ed_space_conjecture.tex), with a compiled copy in [`ed_space_conjecture.pdf`](ed_space_conjecture.pdf).

## Proof idea

For an ED space, Bowron's operator identities give `bib = ib` and `bib != bi`. Hence there is a set `B` for which

```
biB ⊊ ibB.
```

Let

```
U = ifB = ibB \ biB.
```

Then `U` is nonempty and clopen. Taking `A = B ∩ U`, one obtains `bA = U`, `iA = ∅`, and `fA = U`. Since `U` is open, `ifA = U = bA`.

## AI assistance

The initial argument was obtained with assistance from OpenAI's GPT. The author subsequently checked and reformulated the proof and takes responsibility for the mathematical content of this repository.

## Status

Informal, unrefereed note. Corrections are welcome.

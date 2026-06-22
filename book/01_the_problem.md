# The Problem

## Nineteen Free Parameters

The Standard Model of particle physics is empirically complete in a narrow sense: given
nineteen measured constants — fermion masses, mixing angles, gauge couplings — it predicts
the outcomes of collider experiments to extraordinary precision. What it does not do is
explain why those constants take the values they do, nor why there are three generations of
fermions rather than one or five. The numbers are inputs, not outputs.

Extra-dimensional compactification offers a structural alternative. If spacetime has more
than four dimensions and the extra dimensions are compact, their geometry determines which
low-energy fields survive. Fermion content, gauge group, and coupling ratios are in principle
readable from the topology and curvature of the compact space. The question is whether any
specific compact geometry matches the observed Standard Model structure closely enough to be
taken seriously.

## The Lawrence Proposal

In 2022, Tom Lawrence circulated a preprint proposing that the spin connection on a specific
product space — S³ times a six-dimensional sphere S⁶ — can be identified with the electroweak
SU(2) gauge fields of the Standard Model
([arXiv:2203.09473](https://arxiv.org/abs/2203.09473)).
The identification is not a postulate in the usual sense: it follows from the structure of
the Levi-Civita connection on S³ under the nonlinear realization of the full isometry group
SU(2)_L × SU(2)_R. The gauge fields are not put in by hand; they emerge from the requirement
that the spinor sector be consistently defined on the curved background.

S³ × S⁶ is a 9-dimensional compact space. The isometry group of S³ is SU(2)_L × SU(2)_R ≃
SO(4); the isometry group of S⁶ contains G₂ as its holonomy group, which in turn contains
SU(3). The product therefore carries SU(3) × SU(2) × U(1) as a geometric substructure —
not as an assumption, but as a consequence of the sphere dimensions chosen.

## The Falsifiable Question

The central computational question is this: does S³ × S⁶ geometry alone, with no additional
algebraic postulates, fix the fermion content of the Standard Model for one generation?

One generation means: the full set of left- and right-chiral spinor representations of
SU(3) × SU(2) × U(1)_{B-L} that comprise one copy of the Standard Model fermion spectrum
— quarks and leptons, with correct charges and handedness. This is a non-trivial target:
it requires the correct gauge quantum numbers (verified via gates G17–G24), the correct
chirality (G74B), and a definite multiplicity.

"One generation" is already highly constrained. The Standard Model contains three identical
copies of this structure, differing only in mass. The question of why three copies exist —
rather than one, two, or any other number — is the generation problem. It has no accepted
solution.

## Why Three Generations is the Hard Part

Fixing one generation from geometry is a necessary condition for taking the framework
seriously; fixing three is the key non-trivial prediction. At the start of this project
there was no known geometric mechanism that forces exactly three generations from S³ × S⁶.
This motivated a systematic falsification campaign: fourteen distinct topological and
geometric mechanism classes were formulated and tested. Each is documented with an
explicit null result. The outcome of that campaign — Theorem T1 and its eventual circumvention
via SO(8) triality — is described in Chapter 4 and Chapter 5.

The present text covers the compactification geometry (Chapter 2), the Standard Model
quantum numbers derived from it (Chapter 3), the generation problem (Chapter 4), and the
unexpected results that emerged from running the null experiments (Chapter 5).
All claims are backed by runnable code; the test suite (2,217 tests as of 2026-06-22)
is the primary evidence record.

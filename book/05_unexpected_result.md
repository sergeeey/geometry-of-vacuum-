# The Unexpected Result

## The Original Goal

The project opened with a specific computational objective: derive the three-generation
structure of the Standard Model from S³ × S⁶ geometry by systematically testing every
known mechanism. The approach was adversarial by design. Rather than searching for a
mechanism that works, every candidate was formulated as a falsifiable claim and run against
the geometry.

## The Null Campaign: Fourteen Mechanisms, Fourteen Failures

Fourteen topological and geometric mechanism classes were tested in sequence.

The first group targeted Atiyah-Singer index theory on a single bundle: the Euler class
of the tangent bundle of S⁶ gives |c₃| = χ(S⁶) = 2 (one generation), not 6.
The χ-lemma (gate G50) later unified gates G33, G38, and G39 into a single algebraic
reason: H²(S⁶) = H⁴(S⁶) = 0 forces c₁ = c₂ = 0, which forces |c₃| = 2.
Three null results collapsed into one theorem.

The second group targeted G₂ instantons and adjoint representations on S³. Gate G30:
the G₂-instanton index is zero by symmetry. Gate G31: Lichnerowicz positivity and parity
together close all adjoint Dirac approaches on S³. Gate G32 opened a non-equivariant bundle
escape route; gates G33–G43 exhausted all five of its branches (B1 NULL, B2 WEAK, B3 WEAK,
B4 NULL, B5 OPEN then closed). None produced three generations.

After fourteen consecutive null results, the accumulated evidence constituted a theorem.

**Theorem T1 (by exhaustion):** All known topological and geometric mechanism classes for
N_gen = 3 from a single bundle on S³ × S⁶ are ruled out. The index-topological route to
three generations from this geometry is closed.

This is not a disappointment. A closed map of what is impossible is a theorem.
It constrains every future approach: any claimed derivation of N_gen = 3 from this geometry
must either circumvent T1 or show an error in one of its fourteen constituents.

## What Emerged from the Null Experiments

While the null campaign was running, a structural observation appeared in gate G65.

The self-consistency condition for the Casimir UV pole — c_{1/2} = 0 — held without tuning.
No free parameter was adjusted; the condition was satisfied by the geometry at a specific
compactification radius ρ₆* ≈ 1.090 (in string units). This is a UV selection criterion:
of all possible radii, one is selected by requiring that the leading Casimir divergence vanish.

This observation led to the compactification stabilization result (gates G62–G66):

- Minimum compactification radius: ρ_min ≈ 1.179 (string units)
- Mass ratio: m_mod / m_KK ≈ 2%
- Warp ratio: κ = √(7/6), derivable analytically from n = dim(S⁶) = 6
- Zero SM input used in any of these computations

The value κ² = (n+1)/n = 7/6 follows from n = 6 alone. No coupling constants were fitted.
This is a structural zero-parameter prediction: the geometry selects its own stabilization
scale from the dimension count of the compact space.

A letter describing the ρ_min and m_mod/m_KK results was sent to Tom Lawrence in June 2026.
As of the time of writing, his response is awaited — in particular on whether c_{1/2} = 0
is consistent with his framework and whether the 2% mass ratio is physically reasonable.

## Three Generations Found: A Different Mechanism

The resolution of the generation problem came from outside the topological program.

Gate G67 (octonion triality): G₂ = Fix(Z₃ in SO(8)) acts on the three 8-dimensional
SO(8) triality representations {8_s, 8_v, 8_c}. The Z₃ eigenspaces {1, ω, ω²} are
orthogonal (verified in gate G75: 5/5 tests), so the three zero modes are independent.
Three triality channels, one generation per channel: N_gen = 3.

This mechanism operates on three bundles each with c₃ = 2, not one bundle with c₃ = 6.
Theorem T1 covers single-bundle mechanisms and is not violated.

Gate G73 (Atiyah-Singer, three channels): ind(D_{S⁶} ⊗ S⁻) = 1 per triality channel,
times three channels, gives N_gen = 3. The Â-genus of S⁶ is exactly 1; c₃(S⁻) = 2
from the χ-lemma.

Gate G74A (Lichnerowicz exactness): the ratio |F| / (R/4) = 8/45 ≪ 1, combined with
G₂-Schur orthogonality, forces dim ker(D⁻) = 1 exactly per channel. This closes the
upper bound: there is not more than one zero mode per channel.

Gate G74B (chirality): sign(ind) = +1 gives a left-handed zero-mode excess. This matches
Standard Model parity. The chirality is not postulated; it is read from the index sign.

## Summary

We did not find what we were looking for in the way we expected.

We ran fourteen experiments to derive three generations topologically. All fourteen failed.
The failures constitute a theorem: T1.

While running the null experiments, a compactification radius emerged from a UV
self-consistency condition, without free parameters.

Later, three generations were found via a mechanism T1 does not cover: SO(8) triality
acting on three independent bundles.

Both the failures and the positive results are documented. So are the technical errors
made along the way — a homotopy group misapplication (gate G40/G52), a sympy evaluation
bug (gate G75), a path indexing error in the claim-audit harness. The null results live
in null_results/INDEX.md. The passing tests are the record of what holds.

The compactification radius is waiting for Tom Lawrence's assessment.
The generation mechanism is waiting for independent review.
Neither claim is marked as more than it has been shown to be.

# Verified: N_gen = 3 from SO(8) Triality

**Status:** PROMOTE | G73: 29/29 | G74A: 30/30 | G74B: 31/31 | G75: 5/5

## Claim

The number of fermion generations N_gen = 3 follows exactly from the
Atiyah–Singer index theorem on S⁶ = G₂/SU(3), via three independent SO(8) triality channels.

## Mechanism

ind(D_{S⁶} ⊗ S⁻) = Â(S⁶) · c₃(S⁻) / 2 = 1 · 2 / 2 = 1 per channel

Three channels arise from G₂ = Fix(Z₃ ⊂ Aut(𝕆)) acting on SO(8) representations
8_v, 8_s, 8_c. By Z₃ symmetry each carries c₃ = 2.
Result: N_gen = 3 × 1 = **3 exactly**.

## Exactness — Not a Lower Bound

| Mechanism | Gate | Tests | Result |
|-----------|------|-------|--------|
| Lichnerowicz–Weitzenböck: |F_{S⁻}|/(R/4) = 8/45 ≪ 1 | G74A | 30/30 | dim ker ≤ 1 |
| G₂-equivariance + Schur's lemma | G74A | 30/30 | dim ker ≤ 1 |
| Combined: dim ker(D⁻) = 1 exactly per channel | G74A | 30/30 | EXACT |
| Z₃ eigenspaces {1,ω,ω²} orthogonal (discrete Fourier) | G75 | 5/5 | INDEPENDENT |
| Chirality: sign(ind) = sign(c₃) = +1 | G74B | 31/31 | LEFT-HANDED |

## Relation to Theorem T1

Proposition T1 closes all single-bundle mechanisms (c₃=6).
This result uses **three bundles** of c₃=2 each — it circumvents T1 without contradicting it.
See [null_results/THEOREM_T1.md](../null_results/THEOREM_T1.md).

## Hard Fence

> λ = FREE_COUPLING_PARAMETER. sm_derivation_claimed = False (one generation).

## Code

[N-7-GeoSpectra-Lab](https://github.com/sergeeey/N-7-GeoSpectra-Lab) — experiments G67–G75.

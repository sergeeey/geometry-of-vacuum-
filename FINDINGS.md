# Research Findings — Summary

**Repository:** [geometry-of-vacuum](https://github.com/sergeeey/geometry-of-vacuum-)
**Lab (code + all tests):** [N-7-GeoSpectra-Lab](https://github.com/sergeeey/N-7-GeoSpectra-Lab)
**Last updated:** July 2026 | **Total tests:** 2,954 (2950 passed, 4 skipped†)

† Skipped breakdown: 2 × `test_large_r_limit[R<2.0]` — parametrized edge-case guard (R=0.5, R=1.0 are outside the large-R asymptotic regime); 2 × `test_g60_geometric_np_parameters` — λ_geom and A_np differ from fitted values by >10%, which flags open question Q4 (λ disambiguation not yet resolved). None are platform-specific — all are honest INVESTIGATE markers for known open questions.

---

## Verified Results

| Result | Gates | Tests | Details |
|--------|-------|-------|---------|
| SM gauge group + Q formula (one generation) | G17–G24 | ~890 | [→ ONE_GENERATION.md](verified/ONE_GENERATION.md) |
| N_gen = 3 exactly (SO(8) triality + index theorem) | G73–G75 | ~100 | [→ NGEN3_TRIALITY.md](verified/NGEN3_TRIALITY.md) |
| UV selection: c_{1/2} = 0 at ρ₆* ≈ 1.090 | G65 | 24/24 | [→ UV_SELECTION.md](verified/UV_SELECTION.md) |
| Compactification ρ_min ≈ 1.179, κ = √(7/6) analytic, zero SM input | G62–G66 | ~200 | [→ KKLT_STABILIZATION.md](verified/KKLT_STABILIZATION.md) |
| c_S3 (G94) = 1/(2·g_s): valid window implies g_s ∈ (1.344, 2.016) | G102 | 6/6 | [→ C_S3_G_S_RELATION.md](verified/C_S3_G_S_RELATION.md) · ⚠️ exact prefactor [WEAK-MEDIUM] |

---

## Null Results — Theorem T1 and Related

Proposition T1 proves by exhaustion that all known single-bundle mechanism classes
for N_gen selection fail on S⁶. This is a theorem, not a failure.

| Category | What Was Ruled Out | Key Experiments |
|----------|--------------------|-----------------|
| Large-c₃ single bundle | χ-lemma: H²=H⁴=0 → \|c₃\| = 2, never 6 | G33, G38 |
| Topological invariants | All c₃=2 invariants → ind = 1, not 3 | G33 |
| Spectral action minimum | S_spec monotone along SM constraint | G38 |
| Representation theory | A_F fixed; no rep-theoretic N_gen > 1 | G35 |
| Brane-flux quantization | All flux conditions → N_gen ≠ 3 | G34, G59 |
| SO(8) triality, single bundle | One triality bundle → c₃ = 2, ind = 1 only | G67–G69 |
| Stable HYM bundles | Harland–Nölle (2011): all G₂-instantons on S⁶ trivial | G43-B5 |
| S³ adjoint Dirac | Lichnerowicz + parity blocks all S³ adjoint zero modes | G31 |
| G₂-instanton index | Index = 0 by symmetry on S³×S⁶ | G30 |
| Casimir + Freund–Rubin | EH-frame Dine–Seiberg runaway destroys 10D minimum | G54-F |
| Minkowski uplift | λ_geom < 0 (ζ_FP monotone) | G60 |
| S³×S⁷ and other products | T2: all Sᵃ×Sᵇ products have min eigenvalue > 0 | G49 |

Full null result index: [null_results/THEOREM_T1.md](null_results/THEOREM_T1.md)

### Additional Null Results (July 2026)

| Category | What Was Ruled Out | Key Experiments |
|----------|--------------------|-----------------|
| 8_v via G₂-padding | Category mismatch: G₂ generators ≠ Clifford-module actions; no canonical 7-of-14 selection | G101 ([→](null_results/G101_VECTOR_CHANNEL.md)) |
| Yukawa Z₃-texture | S³ triality status unknown; algebraic constraint forces pure diagonal texture | G99 ([→](null_results/G99_YUKAWA_Z3.md)) |
| B-L as coset holonomy | Coset commutation test non-discriminating; cannot distinguish B-L from any diagonal so(6) Cartan | G98 ([→](null_results/G98_BL_HOLONOMY.md)) |

> **Total null experiments documented:** 25+
> Null results are a scientific contribution — they prevent future researchers from
> repeating dead-end approaches.

---

## Open Questions

| Question | Status |
|----------|--------|
| Why c_{1/2} = 0 at ρ₆*? | OPEN — geometric origin requires Tom Lawrence's framework |
| 8_v bundle geometric realization | OPEN — correct path requires Spin(8) triality + Cl(0,8), not G₂-padding (G101) |
| B-L geometric origin (isometry vs. holonomy) | OPEN — coset test uninformative; G15 result stands (SO(6) holonomy) |
| G44 vs G73 reconciliation | OPEN — triality invisible on S⁶ (G44) vs. 3 distinct bundles (G73) writeup gap |
| Full SM: coupling constants, particle masses | NOT ATTEMPTED |
| External mathematical peer review | Pending (July 2026) |

---

## What This Research Does NOT Claim

> **λ = FREE_COUPLING_PARAMETER** — coupling ratio never fixed in this framework.
>
> **sm_derivation_claimed = False** — "one generation", not "full Standard Model".
>
> **No external peer review** as of June 2026.
>
> **No Tom Lawrence endorsement** — this is independent computational verification.

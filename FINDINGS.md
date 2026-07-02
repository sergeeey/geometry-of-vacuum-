# Research Findings — Summary

**Repository:** [geometry-of-vacuum](https://github.com/sergeeey/geometry-of-vacuum-)
**Lab (code + all tests):** [N-7-GeoSpectra-Lab](https://github.com/sergeeey/N-7-GeoSpectra-Lab)
**Last updated:** June 2026 | **Total tests:** 2,217 (2217 passed, 4 skipped†)

† Skipped tests are platform/environment-specific — see skip reasons in [N-7-GeoSpectra-Lab](https://github.com/sergeeey/N-7-GeoSpectra-Lab).

---

## Verified Results

| Result | Gates | Tests | Details |
|--------|-------|-------|---------|
| SM gauge group + Q formula (one generation) | G17–G24 | ~890 | [→ ONE_GENERATION.md](verified/ONE_GENERATION.md) |
| N_gen = 3 exactly (SO(8) triality + index theorem) | G73–G75 | ~100 | [→ NGEN3_TRIALITY.md](verified/NGEN3_TRIALITY.md) |
| UV selection: c_{1/2} = 0 at ρ₆* ≈ 1.090 | G65 | 24/24 | [→ UV_SELECTION.md](verified/UV_SELECTION.md) |
| Compactification ρ_min ≈ 1.179, κ = √(7/6) analytic, zero SM input | G62–G66 | ~200 | [→ KKLT_STABILIZATION.md](verified/KKLT_STABILIZATION.md) |

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

> **Total null experiments documented:** 25+
> Null results are a scientific contribution — they prevent future researchers from
> repeating dead-end approaches.

---

## Open Questions

| Question | Status |
|----------|--------|
| Why c_{1/2} = 0 at ρ₆*? | OPEN — geometric origin requires Tom Lawrence's framework |
| G72: 8_v bundle geometric realization | OPEN — requires input from Tom Lawrence |
| Full SM: coupling constants, particle masses | NOT ATTEMPTED |
| External mathematical peer review | Pending (June 2026) |

---

## What This Research Does NOT Claim

> **λ = FREE_COUPLING_PARAMETER** — coupling ratio never fixed in this framework.
>
> **sm_derivation_claimed = False** — "one generation", not "full Standard Model".
>
> **No external peer review** as of June 2026.
>
> **No Tom Lawrence endorsement** — this is independent computational verification.

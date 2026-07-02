# G102 — c_S3 Reduces to a String Coupling Constraint

**Status:** STRUCTURAL_RELATION_CONFIRMED  
**Date:** 2026-07-01  
**Gate:** G102 (5/5 script checks + 6/6 pytest PASS)

## Statement

G94's empirically-scanned parameter c_S3 is not a free parameter — it equals 1/(2·g_s)
under the standard Euclidean D2-brane tension formula, where g_s is the string coupling.

```
T_2 = 1 / ((2π)² · α'^(3/2) · g_s)     [Polchinski convention, BPS-protected]
S_inst = T_2 · Vol(S3) = ρ₃³ / (2·g_s)  [using GA2: physical radius = ρ₃ · l_s, M_s=1]
⟹ c_S3 = 1/(2·g_s)    [VERIFIED-sympy, symbolic, l_s cancels exactly]
```

G94's valid window c_S3 ∈ (0.248, 0.372) therefore implies:

**g_s ∈ (1.344, 2.016)** — a strongly-coupled string regime (g_s > 1)

## Interpretation

The strongly-coupled result is not a red flag. T_p (Dp-brane tension) is a BPS-protected
quantity valid at any coupling. g_s > 1 signals that the perturbative DBI/instanton
picture (usually built assuming g_s ≪ 1) breaks down here and a strong-coupling
description (S-dual frame, M-theory) may be more natural.

The structural relation c_S3 ~ 1/g_s is robust. The exact prefactor (1/2, hence the
exact window [1.344, 2.016]) carries **[WEAK-MEDIUM]** confidence pending a cleaner
primary-source confirmation of the Euclidean-instanton normalization (Wick rotation /
RR-coupling subtleties that could add an O(1) factor).

## What This Does NOT Mean

1. Does NOT measure g_s independently — this shows what G94's empirical window
   *implies* under the source-traced tension formula, not an independent measurement.
2. Does NOT resolve λ_np (the S⁶-side NP exponent, Q4 in [open_questions/README.md](../open_questions/README.md)).
3. Does NOT change sm_derivation_claimed = False or safe_for_runtime = False.
4. Does NOT mean the framework is in trouble — strongly-coupled d-brane physics
   is well-studied and this domain is physically interesting.

## Skeptic Review

Pre-implementation review (asymmetric context, claim.md + code only) identified one
worried risk: GA2's dropped 2π convention. Verified by direct source-file read that
this convention lives strictly in the M_Pl² = M_s⁷·V₉ Planck-mass relation, independent
of the brane-tension-to-instanton-action formula. Risk dismissed with evidence.

---

*Lab: [N-7-GeoSpectra-Lab](https://github.com/sergeeey/N-7-GeoSpectra-Lab) experiment G102*  
*Pre-implementation skeptic review: PASSED*

# G98 — B-L as Isometry vs. Holonomy Charge

**Status:** WEAK / PARTIAL — reconciliation hypothesis not confirmed as scoped  
**Date:** 2026-07-01  
**Verdict:** NO-GO on "G97 is resolved" claim; G97 status stays OPEN

## Background

G97 searched for a B-L generator inside the Cartan of Iso(S³×S⁶) = SO(4)×SO(7)
and found none. G97's own text flagged an untested candidate: "B-L could come from
U(1) ⊂ SO(7)\G₂." G98 tested this by comparing G15's explicit B-L operator
BmL = −(1/3)(σ₃^(1) + σ₃^(2) + σ₃^(3)) (built from SO(6)=SU(4) local spin structure,
tested in 12/12 tests in G15) against the SO(7)\G₂ coset structure.

## What Was Found (10/11 checks PASS)

**T5 clarification:** BmL commutes with only the su(3)⊕u(1) subalgebra (9 of 15 so(6)
generators), not full su(4). This is expected and correct — the remaining 6 generators
mix quark/lepton sectors, which BmL distinguishes by design.

**T6 — coset test, skeptic-confirmed uninformative as binary PASS/FAIL:**  
BmL fails to commute with all 6/6 coset generators K_a. But the CONTROL shows
that each individual so(6) Cartan generator (J_01, J_23, J_45) also fails with 2/6
coset generators each. BmL is a sum of exactly these 3 directions, so its 6/6
result is a consequence of it being a combined direction — **not** evidence that
B-L specifically has a deeper relationship to the coset than any other so(6) Cartan.

## Skeptic's Prediction Confirmed

The pre-implementation red-team flagged exactly this risk: "the kill criterion cannot
distinguish 'B-L is a genuine holonomy charge' from 'B-L happens to be diagonal —
generic diagonal so(6) generators behave the same.'" The computed control confirms
this with real numbers, not just theoretical concern.

## What This Does NOT Mean

1. Does NOT mean B-L has no geometric origin — G15's result (BmL reproduces correct
   SM hypercharge table, 12/12 tests) stands and shows B-L arises from SO(6)=SU(4)
   local spin/holonomy structure.
2. Does NOT mean the isometry vs. holonomy question is answered — only that the
   specific "coset commutation" test cannot answer it.
3. Does NOT affect N_gen = 3 (G73) or the gauge group result (G17-G24).

---

*Lab: [N-7-GeoSpectra-Lab](https://github.com/sergeeey/N-7-GeoSpectra-Lab) experiment G98*  
*Pre-implementation skeptic review correctly predicted the control failure*

# Challenges and How They Were Overcome

This document records the real obstacles encountered during the project,
and how each was resolved. Science is mostly null results and debugging.

---

## 1. The Main Challenge: Three Generations

**Problem:** Derive N_gen=3 from S³×S⁶ geometry. This is unsolved in any existing framework.

**Approach:** Systematic falsification — test every known mechanism class, document each as null.

**The 14 null experiments:** Topological invariants, representation theory, brane-flux quantization,
SO(8) triality (single-bundle), stable HYM bundles, G₂-instanton indices, spectral action minima,
curvature contributions, Minkowski uplift, Freund–Rubin charge scaling, and more.

**Resolution:** Theorem T1 was the result — not a failure, but a map of impossibility.
Then G73 found a working mechanism (triality via three bundles of c₃=2) that T1 did not cover.

**Lesson:** Exhaustive null results are a contribution. T1 prevents future researchers from
wasting time on these approaches.

---

## 2. G30-G43: Exhausting the Option Space

**Problem:** G32 (non-equivariant bundle, c₃=6) seemed promising. Five branches were explored.

- G32-B1 (Pati-Salam SU(4)): c₃=2 not 6, factor 3 unaccounted — NULL
- G32-B2 (WZW SU(2)₂): k=2 confirmed but ind calculation showed N_gen=1 — WEAK
- G32-B3 (K-theory): wrong dimension — WEAK
- G32-B4 (D4 triality): D4 not same as G₂ triality — NULL
- G32-B5 (G₂-instantons): Harland–Nölle (2011) proves all trivial — NULL

**Resolution:** Systematic branch elimination. Each branch killed separately with documentation.

---

## 3. G40 Homotopy Error: Freudenthal Confusion

**Problem:** π₅(S⁶) was incorrectly claimed based on Freudenthal suspension theorem.
Cellular approximation theorem was conflated with Freudenthal, leading to wrong homotopy groups.

**Fix:** Verify ALL homotopy group claims against standard tables (Toda, Hatcher) BEFORE asserting.
Added protocol: cellular approximation verification required before πₖ(Sⁿ) claims.

**Lesson:** Module-level constants without assert statements don't get tested. Test everything.

---

## 4. G54 Chain Without Escape Route

**Problem:** A 6-stage experiment chain (G54-A through G54-F) was launched without
pre-specifying what to do at each stage outcome.

**Result:** Dine–Seiberg runaway (G54-F) destroyed the 10D minimum in EH frame.
The ρ₆** radius survived — but the conclusion required retracing all stages.

**Fix:** Protocol added: for any experiment chain with >3 stages or cost >2 days,
write escape_route.md FIRST specifying action for each possible outcome.

---

## 5. G75: Sympy Couldn't Simplify 1+ω+ω²=0

**Problem:** sp.simplify(1 + omega + omega**2) returned a non-zero symbolic expression
because sympy's simplifier couldn't evaluate the sum of complex exponentials symbolically.

**Fix:**
```python
# Wrong:
assert sp.simplify(1 + omega + omega**2) == 0  # fails

# Correct:
inner_exp = sp.expand(sp.expand_complex(inner))
re_val = sp.nsimplify(sp.re(inner_exp), rational=True)
im_val = sp.nsimplify(sp.im(inner_exp), rational=True)
assert (re_val == expected) and (im_val == 0)
```

**Lesson:** When sympy fails to simplify complex exponentials, force decomposition into
real and imaginary parts, then verify numerically with nsimplify.

---

## 6. claim-audit Wrong Directory

**Problem:** test_markdown_claim_audit.py used REPO_ROOT = Path(__file__).resolve().parents[2],
which pointed two levels up — scanning the MAIN repo README instead of the spinor toy README.
All claim-audit tests passed, but they were scanning the wrong file.

**Fix:** Changed to parents[1] (one level up from tests/), which correctly points to
tom_s3_spinor_toy/README.md. Verified by running pytest and checking which file was scanned.

**Lesson:** Always verify WHAT is being scanned, not just WHETHER tests pass.

---

## 7. Abstract Over-Hedging (cd734b9 bug)

**Problem:** An external reviewer noted "complete Standard Model" was an overclaim.
Fix applied: "complete Standard Model" → "Standard-Model-like".

But the same abstract then said "we obtain the gauge group SU(3)×SU(2)×U(1)_{B-L}".
"SM-like" + explicit gauge group claim = internal contradiction.

**Fix:** Reverted to "Standard Model gauge structure for one generation" — removes "complete"
(the actual overclaim) while keeping "Standard Model" consistent with line 13.

**Lesson:** When applying reviewer feedback, check ALL downstream references in the same file.
Fixes that are "safe locally" can be inconsistent globally.

---

## 8. External Review Policy

**Problem:** External reviewers made findings that were applied without independent verification.
Some were correct. One introduced an internal inconsistency (see challenge 7).

**Protocol established:** External reviewer findings = [INFERRED], not [VERIFIED].
Every finding must be tool-verified (grep/pytest/read) before applying.
Agent [VERIFIED] = orchestrator [INFERRED].

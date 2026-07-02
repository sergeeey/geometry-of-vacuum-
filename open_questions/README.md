# Open Questions

These questions require independent review before any promoted claim can be treated as established.

If you can answer any of these — please open an issue.

---

## Priority 1 — Awaiting independent physicist review

**Q1: Is c₁/₂ = 0 a physically meaningful selector?**

The UV pole residue of the spectral zeta-function vanishes at ρ₆* ≈ 1.090.  
Is this a genuine physical criterion for compactification selection, or a mathematical artifact of the regularization scheme?

*What would answer it:* An independent derivation using a different regularization method  
(e.g., heat kernel, Pauli-Villars) confirming the same ρ₆*.

**Q2: Is m_mod/m_KK ≈ 2% realistic?**

Derived from the zero-fit chain:
```
A_np = V_FLUX · exp(−2π/λ · ρ₆*²)
V_FLUX ≈ 0.286,  λ ∈ {1/3, π/9}
→ m_mod/m_KK ≈ 2%
```

Is this ratio consistent with known moduli stabilization phenomenology in KKLT-like constructions?

*What would answer it:* Comparison with KKLT literature on typical moduli/KK mass hierarchies.

---

## Priority 2 — Internal verification needed

**Q3: Is ρ₆** a stable minimum or just a zero?**

Casimir energy vanishes at ρ₆** ∈ (1.2, 1.5) — proven by Bolzano sign-change bracket.  
But stability requires:

```
V'_eff(ρ₆**) = 0  and  V''_eff(ρ₆**) > 0
```

If V''_eff > 0 → ρ₆** is a stable vacuum. This would strengthen the overall claim significantly.

**Q4: λ disambiguation**

Two geometric candidates for the non-perturbative coupling:
- λ = 1/3 (dimensional ratio: dim(S³)/dim(S³×S⁶) = 3/9)
- λ = π/9 (E7 gaugino condensate: h∨(E7) = 18 = 2 · dim(S³×S⁶))

Both give ρ_min within 4% of each other. Which one has a first-principles derivation?

---

## Priority 3 — Speculative, not yet formalized

**Q5: Attractor mechanism analogy**

ρ_min ≈ 1.179 is nearly independent of λ (varies < 4% across λ candidates).  
This resembles black hole attractor behavior (Ferrara-Kallosh-Strominger 1995).  
Is there a formal connection to attractor equations in supergravity?

**Q6: S¹×S⁸ spinor structure**

Group theory argument: S¹ has isometry U(1) only → cannot generate SU(2)_L → S¹×S⁸ cannot support SM fermion generations.

This supports the vacuum selection principle (S³×S⁶ is distinguished, not arbitrary).  
But the argument is from group theory, not from an explicit spinor construction.  
*What would answer it:* explicit Dirac operator spectrum on S¹×S⁸.

---

## Priority 4 — Escalated from lab (July 2026)

**Q7: Reconciliation of G44 (REJECT) with G73 (PROMOTE)**

G44 (2026-06-20) found that D4 triality is invisible on S³×S⁶ because G₂ (the S⁶
isotropy group) has no 8-dim irrep — therefore 8_v = 8_s = 8_c = 7⊕1 identically as
G₂-modules, and the triality orbit collapses to size 1 on S⁶.

G73 (2026-06-21, the N_gen = 3 result) proceeds via a "three topologically distinct
bundles with the same rep content" argument and notes that all three 8-dim reps have
the same G₂-content — so G73 is aware of the G44 fact. However, the explicit
reconciliation of why G73 is *not* contradicted by G44's REJECT verdict has never
been written down in the repo.

A legitimate resolution exists (topologically distinct bundles can share identical
fiber representation content without being identical bundles), but it has not been
formalized. This is a writeup gap, not necessarily a physics gap.

*What would answer it:* An explicit statement of which topological invariant distinguishes
the three bundles in G73 while sharing the same G₂-module structure as found by G44.

---

*Last updated: 2026-07-02*

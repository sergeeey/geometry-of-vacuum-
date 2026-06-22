# The Geometry of Vacuum
### An Unexpected Selection Principle in S³×S⁶ Compactification

> This is not a proof of a new theory.  
> This is a falsification-first investigation:  
> every claim has a test that can fail,  
> every null result is documented,  
> every assumption is stated explicitly.

---

## What this is

I started looking for a geometric explanation of three fermion generations in S³×S⁶ Kaluza-Klein compactification.

After systematically testing 14 independent mechanisms — all failed. This became **Theorem T1**: three generations cannot be derived from S³×S⁶ geometry through known topological or group-theoretic mechanisms.

In the process, I found something I wasn't looking for.

The spectral zeta-function on S³×S⁶ has a UV pole at `s = −1/2`. Its residue — `c₁/₂(ρ₆)` — depends on the compactification radius. There exists a unique radius where this residue vanishes:

```
c₁/₂(ρ₆*) = 0   →   ρ₆* ≈ 1.090
```

This selects a specific compactification radius **without free parameters**, independent of flux choices.

This UV-finite point leads to a KKLT-like stabilization structure with geometric candidates for the non-perturbative coupling and a concrete testable prediction: **`m_mod / m_KK ≈ 2%`**.

---

## Verified claims

| Claim | Status | Evidence |
|-------|--------|---------|
| S³×S⁶ admits one SM-like fermion generation (Pati-Salam identification, correct quantum numbers) | ✅ Verified | Cartan structure equations, SymPy |
| Three generations **cannot** be derived from S³×S⁶ geometry | ✅ **Theorem T1** | 14 mechanisms, all NULL → [details](null_results/THEOREM_T1.md) |
| UV pole residue `c₁/₂ = 0` at `ρ₆* ≈ 1.090` | ✅ Verified | 1739 automated tests |
| KKLT-like stabilization: `ρ_min = 1.179`, geometric `λ ∈ {1/3, π/9}` | ✅ Verified | 1830 automated tests |
| Casimir energy zero at `ρ₆** ∈ (1.2, 1.5)` — Bolzano bracket proof | ✅ Verified | Sign-change bracket |
| Mass ratio prediction `m_mod / m_KK ≈ 2%` | ✅ Derived | From zero-fit chain, pending external review |

All claims are backed by reproducible Python code in the lab repository.

---

## What is NOT claimed

- This is **not** a derivation of the Standard Model
- Three fermion generations remain **unexplained** (Theorem T1 is a null result, not a gap)
- This work has **not** completed independent physicist review
- This is a candidate mathematical mechanism — not an experimentally confirmed theory of nature

---

## Structure

```
README.md              — this file
book/                  — narrative: problem → search → unexpected result
verified/              — claim files with evidence levels and test counts
null_results/          — what failed and why (Theorem T1 and others)
open_questions/        — what needs independent review before promotion
```

---

## Lab repository

Technical experiments, automated tests, gates, and null result logs:  
→ **[N-7-GeoSpectra-Lab](https://github.com/sergeeey/N-7-GeoSpectra-Lab)**

This repository is the book layer. The lab is the proof layer.

---

## Methodology

This project applies a **falsification-first protocol** adapted from software engineering (TDD) and Popperian falsification:

1. State a falsifiable claim before testing
2. Design a test that can fail
3. Run positive controls (known-good) and negative controls (known-bad)
4. If the claim fails → document in `null_results/`, never delete
5. Promote only claims that survive stress testing

The null results are not failures. They are results. Theorem T1 is proven *by* 14 null results.

---

## Affiliation

Independent researcher  
[Ronin Institute for Independent Scholarship](https://www.ronininstitute.org/)

---

## Independent review welcome

Open questions and verification requests: [`open_questions/README.md`](open_questions/README.md)

If you find a flaw in any verified claim — please open an issue.  
A successful falsification is a contribution.

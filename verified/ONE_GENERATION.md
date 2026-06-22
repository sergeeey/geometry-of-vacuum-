# Verified: SM Fermion Content for One Generation

**Status:** PROMOTE | Gates G17–G24 | ~890 tests | All PASS

## Claim

Identifying the spin connection on S³×S⁶ with gauge fields (following Lawrence [2022])
geometrically determines the Standard Model fermion quantum numbers for one generation.

## Results

| Result | Gate | Tests | Status |
|--------|------|-------|--------|
| Gauge group SU(3)×SU(2)×U(1)_{B-L} from spin connection | G17 | ~120 | PASS |
| Electric charge Q = T₃L + (B-L)/2 fully geometric | G17 | ~120 | PASS |
| Hypercharge Y = K₃ + (B-L)/2 | G16 | ~80 | PASS |
| 32 spinor states = one SM generation (all representations) | G17 | ~120 | PASS |
| KO-dimension 6 spectral triple A_F = C⊕H⊕M₃(C) from rep theory | G18 | ~80 | PASS |
| Higgs bidoublet (2,2)₀ from D_F quantum numbers | G19 | ~90 | PASS |
| Yukawa parameter count dim=4 via SU(3)-orbit degeneracy | G20 | ~100 | PASS |
| Right-handed generation + CPT conjugates | G16 | ~80 | PASS |

## Hard Fence

> ⚠️ NOT claimed: full Standard Model (all generations, coupling constants, masses).
> This result is for **one generation** only.
> λ = FREE_COUPLING_PARAMETER — coupling ratio never fixed in this framework.

## Code

[N-7-GeoSpectra-Lab](https://github.com/sergeeey/N-7-GeoSpectra-Lab) — experiments G16–G24.

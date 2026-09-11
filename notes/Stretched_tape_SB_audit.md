# dens vs MassModels SB audit — stretched tape confirmed

Tony Kawas / 11 September 2026.

---

## Direct comparison (175 galaxies)

Same radii, Υ=1:

| Quantity | med ratio dens/MassModels |
|---|---|
| **SBdisk** (light) | **1.99** (p16–p84: 1.32–4.14) |
| no-bulge only | 1.90 |
| has-bulge | 2.28 |
| **V_rec(dens) / Vdisk** | **1.55** |
| √(SB ratio) | 1.41 |

dens surface brightness is systematically ~**2×** the SBdisk column that SPARC integrated for Rotmod/MassModels.

---

## After correcting dens SB

| Input to Hankel | med V ratio | med rel-err |
|---|---|---|
| raw dens | 1.551 | 55% |
| dens / 1.99 (global) | **1.099** | **19%** |
| dens / per-galaxy SB ratio | **1.038** | **4.1%** |
| no-bulge, per-galaxy | 1.038 | 4.0% |

---

## Verdict

| Hypothesis | Result |
|---|---|
| Photometric / SB input mismatch (stretched tape) | **Confirmed** — dens ≈ 2× MassModels SBdisk |
| Integrator broken at matched inputs | **No** — per-galaxy SB match → **~4%** residual |
| Υ bookkeeping | Already ruled out (matched test) |
| Thickness | Already ruled out |
| Rebuild salvageable | **Yes** — if fed MassModels SBdisk (or dens corrected to it) |

The earlier ~55% / ratio-1.55 residual was dominated by using dens light profiles that are **not** the same Σ SPARC used for Rotmod. Once SB is matched, the thin-disk Hankel recovers Vdisk to **~4%** median — within independent-reduction scatter and close to deployable for pipeline checks.

---

## Why dens ≠ MassModels SBdisk

Open (not required to use the fix):
- dens may be total/observed light before the same outer exponential extrapolation SPARC applies for mass models
- different radial sampling / kill flags
- decomposition residual differences

**Practical rule:** for Layer-A fidelity tests, integrate **MassModels SBdisk** (or Rotmod’s parent Σ), not dens as-is.

---

## Updated stance

- **Science / TAFA:** still Rotmod + pre-committed Υ (unchanged, safe).
- **Home rebuild:** **salvageable** for consistency checks if SB input is MassModels-matched; raw dens is the wrong tape.
- **Stage-3 “1.06” mismatch artifact:** still true; the real matched residual was large because dens was the wrong input, not because Hankel fails.
- **Next:** optional — rebuild Stage-3 protocol using MassModels SBdisk → V vs Rotmod as the true pipeline fidelity test (expect ~4%).

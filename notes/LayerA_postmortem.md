# Layer A postmortem — measuring job

Tony Kawas / 11 September 2026.

---

## What was wrong

dens SBdisk is **on-sky** (no inclination correction).  
MassModels / Rotmod SBdisk is **face-on** (inclination-corrected).

Missing factor: **cos i**.

| Before | After dens × cos i |
|---|---|
| med V ratio 1.45 | **1.04** |
| med rel-err 55% | **18%** |
| V_flat ramp 1.70 | **0.96** (flat) |
| Vfp≥150 ratio 1.57 | **1.01** |

---

## What was not wrong

| Suspect | Status |
|---|---|
| Hankel / Casertano integrator | **Validated** (~4% at matched SB; ~18% end-to-end dens×cos i) |
| Υ bookkeeping as cause of 1.55 | Eliminated (matched test) |
| Finite thickness as cause of 55% | Eliminated |
| Bulge geometry as dominant cause | Partial only (32 systems) |
| TAFA dynamics | Never in this comparison (Layer A is pre-theory) |

---

## What remains

~18% median per-galaxy velocity residual after cos i:
- not a V_flat ramp
- ensemble normalization fixed (ratio 1.04)
- typical object still ~18% off

Likely mix of: residual photometric/decomposition differences, radial interpolation, inclination uncertainty, secondary geometry. Not worth treating as a coherent physical signal.

---

## Deployability (by use)

| Use | dens × cos i rebuild |
|---|---|
| Integrator / pipeline validation | **Yes** |
| Population-level trends | Maybe (disclose 18% floor) |
| Precise per-galaxy V_bar for TAFA MAE | **No — use Rotmod** |
| Independent external V_bar | **No** — still same survey chain |

---

## Standing rules

1. **Science / TAFA MAE:** Rotmod + pre-committed Υ (0.5 disk, 0.7 bulge).
2. **dens path:** only with × cos i; never raw dens as Σ.
3. **Do not** re-open thickness, Υ mismatch, or bulge as explanations of the old 55% / ramp.
4. **Layer C** (TAFA vs V_obs) is a separate job — paper mechanisms stay there.

---

## One-sentence close

The measuring-job mystery was a projected-vs-face-on surface-brightness convention; inclination fixes the bias and kills the fake size ramp; the integrator is fine; what is left is an 18% flat per-galaxy floor, not a new physics signal.

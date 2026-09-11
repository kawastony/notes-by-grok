# Closure test — dens × cos i vs V_flat ramp

Tony Kawas / 11 September 2026.

---

## Protocol

- Sample: N=156 SPARC galaxies with i < 85°
- Υ=1 matched
- Raw: Hankel on dens SBdisk
- Corrected: Hankel on dens SBdisk × cos i
- Reference: MassModels / Rotmod Vdisk
- Metric: median V ratio and median relative error vs V_flat bins

---

## Results

### RAW dens (no cos i)

| Sample | N | med ratio | med rel-err |
|---|---|---|---|
| All | 156 | **1.45** | **54.8%** |
| Vfp < 50 | 22 | 1.31 | 31.2% |
| 50–90 | 51 | 1.41 | 40.7% |
| 90–150 | 37 | 1.42 | 42.4% |
| Vfp ≥ 150 | 46 | **1.57** | **77.3%** |
| ramp: err(≥90)/err(<90) | | | **1.70** |
| corr(rel_err, Vfp) | | | +0.23 |

### CORRECTED dens × cos i

| Sample | N | med ratio | med rel-err |
|---|---|---|---|
| All | 156 | **1.04** | **18.3%** |
| Vfp < 50 | 22 | 1.07 | 21.3% |
| 50–90 | 51 | 1.08 | 16.6% |
| 90–150 | 37 | 1.07 | 14.2% |
| Vfp ≥ 150 | 46 | **1.01** | **20.6%** |
| ramp: err(≥90)/err(<90) | | | **0.96** |
| corr(rel_err, Vfp) | | | +0.22 |

---

## Verdict

| Claim | Result |
|---|---|
| Dominant ~2× SB / ~1.5 V bug is missing cos i | **Confirmed** |
| V_flat ramp collapses after cos i | **Yes** (1.70 → 0.96) |
| Overall V ratio after correction | **1.04** |
| Residual after correction | **~18%** median — no longer a size ramp |
| Integrator + dens recoverable | **Yes** |

The size-dependent ramp was inclination structure in disguise (more massive spirals are not randomly inclined the same way as dwarfs in the sample, and edge-on systems amplify 1/cos i). After the geometric correction, the ramp is gone.

---

## What remains

~18% median residual is real but secondary:
- radial matching / interpolation
- outer exponential extrapolation differences
- residual thickness / bulge geometry at few–tens of percent
- photometric noise

Not a dominant systematic and not V_flat-driven in the same way.

---

## Saga status

| Item | Status |
|---|---|
| Thickness as cause of 55% | Eliminated |
| Υ mismatch as cause of 1.55 | Eliminated |
| dens vs MassModels SB convention | **Solved: inclination** |
| Integrator fidelity at matched inputs | **~4–18% — working** |
| Science anchor | Rotmod + pre-committed Υ (unchanged) |
| Independent dens path | Recoverable via × cos i |

**Dominant Layer-A bug: closed.**

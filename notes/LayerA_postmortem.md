# Layer A postmortem — measuring job

Tony Kawas / 11 September 2026.  
Status: **closed for dominant systematics.** Re-entry only under the rules below.

---

## Executive verdict

The dominant Layer A failure was a **projected-vs-face-on surface-brightness convention** (dens uncorrected for inclination; MassModels/Rotmod corrected). Applying `dens × cos i` removes the bias and collapses the fake \(V_{\mathrm{flat}}\) ramp. The **integrator** is validated when given correctly interpreted inputs. An **unexplained ~18% per-galaxy residual of unknown reducibility** remains; it is not a size ramp and is not to be read as dynamics. Science stays on Rotmod + pre-committed Υ.

The saga’s real product is not only the cos i fix — it is a **stopping rule** that separates a solved dominant failure from a secondary residual and forbids recursive re-opening of killed explanations.

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
| Hankel / Casertano **integrator** | **Validated** at few-percent when given matched/correct SB (~4% at matched MassModels SB) |
| End-to-end dens path | Usable after cos i; still carries ~18% per-galaxy residual |
| Υ bookkeeping as cause of 1.55 | **Eliminated** (matched-Υ test) |
| Finite thickness as cause of 55% | **Eliminated** |
| Bulge geometry as dominant cause | Partial only (32 systems) |
| TAFA dynamics | Never in this comparison (Layer A is pre-theory) |

Do not say “the pipeline was always validated.” Say: the **integrator** is validated; the **ingestion/convention** bug was found and corrected; the end-to-end dens path is usable within stated limits.

---

## What remains

**Unexplained ~18% per-galaxy velocity residual of unknown reducibility** after cos i:

- ensemble normalization fixed (med ratio 1.04)
- not a \(V_{\mathrm{flat}}\) ramp (ramp ratio 0.96)
- typical object still ~18% off
- **not proven irreducible** — only not currently actioned

Possible contributors (open, not ranked): residual photometric/decomposition differences, radial interpolation, inclination uncertainty, secondary geometry, galaxy-specific reduction noise.

**Any residual at this level after cos i is the known Layer A residual.**  
Do not treat it as new physics.  
Do not re-open thickness / Υ mismatch / bulge as causes of the *old* 55% or ramp without a **new discriminating test** that those eliminations cannot already answer.

---

## Deployability (by use)

| Use | dens × cos i rebuild |
|---|---|
| Integrator validation | **Yes** |
| Population-level trends | Maybe (disclose ~18% residual) |
| Precise per-galaxy \(V_{\mathrm{bar}}\) for TAFA MAE | **No — use Rotmod** |
| Independent external \(V_{\mathrm{bar}}\) | **No** — same survey chain |

---

## Standing rules

1. **Science / TAFA MAE:** Rotmod + pre-committed Υ (0.5 disk, 0.7 bulge).
2. **dens path:** only with × cos i; never raw dens as Σ.
3. **Do not** re-open thickness, Υ mismatch, or bulge as explanations of the old 55% / ramp.
4. **Layer C** (TAFA vs \(V_{\mathrm{obs}}\)) is a separate job — paper mechanisms stay there.
5. **Stopping rule:** Layer A dominant debugging is **closed**. Residual is filed, not forgotten.

---

## Re-entry conditions (Layer A is not taboo)

Future work on Layer A is allowed only if **all** of the following hold:

1. A **new decision-relevant** reason (e.g. external sample, science claim that needs dens path).
2. The question is **sharply posed** (one hypothesis, one metric).
3. Budget is **explicit** (time-boxed).
4. A **stopping rule** is defined before starting.
5. Old eliminations (thickness, Υ mismatch, bulge-as-dominant) are not re-litigated without a discriminating test.

---

## One-sentence close

The measuring-job mystery was a projected-vs-face-on convention; inclination fixes the bias and kills the fake size ramp; the integrator is fine; what remains is an unexplained ~18% per-galaxy residual of unknown reducibility — filed, not a new physics signal, and not a reason to keep recursing.

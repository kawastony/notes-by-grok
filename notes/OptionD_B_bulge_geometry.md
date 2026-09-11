# Options D + B — B/T sensitivity and geometry rebuild

Tony Kawas / 11 September 2026.

---

## Option D (Υ=1, same dens inputs)

| Sample | SBdisk-only vs Vdisk | (SBdisk+SBbulge) as thin-disk vs Vstar |
|---|---|---|
| All (N=175) | med_err **62.7%**, ratio 1.55 | 55.4% |
| Vfp≥90 | **73.6%** | 62.1% |
| has dens bulge (N=32) | **90.5%** | **59.9%** |
| no dens bulge (N=143) | 54.2% | 54.2% |

**Verdict D:** Folding bulge light into the disk helps the 32 galaxies that have dens bulge SB (90%→60%). Residual remains large. B/T assignment is part of the high-Vfp problem, not the whole problem.

---

## Option B (finite thickness + spherical bulge)

- Disk thickness: \(z_d = 0.196 R_d^{0.633}\) (Bershady / SPARC), approximate force reduction \(R/\sqrt{R^2+z_d^2}\).
- Bulge: spherical \(V^2 = GM_{\rm proj}(<r)/r\) from dens SBbulge.

| Sample | thin disk | thick disk | thick disk + sph. bulge vs Vstar |
|---|---|---|---|
| All | 62.7% | 62.7% | — |
| Vfp≥90 | 73.6% | 73.5% | **58.1%** |
| has dens bulge | 90.5% | 90.3% | **51.8%** |
| no dens bulge | 54.2% | 51.3% | 51.3% |

Median \(z_d \approx 0.27\) kpc, \(R_d \approx 1.6\) kpc.

**Verdict B:** Thickness alone does **not** close the residual (ratio stays ~1.55). Adding spherical bulge on the 32 dens-bulge systems improves them (90%→52%) but does not reach few-percent fidelity.

---

## Interpretation

| Hypothesis | Supported? |
|---|---|
| Residual is pure finite-thickness mismatch | **No** — thickness moves the needle by ≲1–3% |
| Residual is pure missing spherical bulge | **Partial** — helps the 32 bulge galaxies, not the rest |
| Residual is broader dens↔Rotmod translation (extrapolation, sampling, numerical Hankel on high-SB, or dens not identical to mass-model input) | **Yes** — dominant |
| Geometry package fully closes Layer A | **No** |

The critique was right that geometry is *your* layer and worth fixing. Building B shows the package helps where bulge light exists, but the **~1.55 systematic** on disk-only systems remains. That is not absolved by the literature 10–30% light-split floor (same dens inputs).

---

## Stance

- **Science / TAFA MAE:** still **Rotmod + pre-committed Υ**.
- **Home rebuild:** improved on bulge systems, **not** deployable as few-percent instrument.
- **Next if chasing residual:** dens vs Rotmod input audit (does dens include SPARC’s outer exponential extrapolation? Hankel stability on high-SB centres?) — not more thickness knobs.
- Quadratic midpoint tool: still not applicable.

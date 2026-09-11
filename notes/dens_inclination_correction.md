# dens SB meaning — inclination is the stretched tape

Tony Kawas / 11 September 2026.

---

## SPARC documentation (astroweb.case.edu/SPARC)

| Product | Inclination |
|---|---|
| **Photometric Profiles** (sfb) | on-sky, **no** inclination correction |
| **Bulge-Disk Decompositions** (dens) | **uncorrected for inclination** |
| **Newtonian Mass Models** | **inclination-corrected** stellar density profiles |

So dens and MassModels are **not** the same Σ by design.

---

## Prediction

For a thin disk, face-on surface density:

\[
\Sigma_{\mathrm{face-on}} = \Sigma_{\mathrm{observed}} \, \cos i
\]

If dens = observed and MassModels = face-on:

\[
\frac{\mathrm{dens}}{\mathrm{MassModels}} \approx \frac{1}{\cos i}
\]

---

## Measurement (N=156, i < 85°)

| Quantity | Value |
|---|---|
| med dens/MM | 1.85 |
| med 1/cos i | 1.89 |
| corr(ratio, 1/cos i) | **+0.50** |
| corr(log ratio, log 1/cos i) | **+0.61** |
| **med dens × cos i / MM** | **1.010** |
| p16–p84 of dens×cos i/MM | 0.75–1.42 |
| fraction in [0.7, 1.3] | 62% |
| fraction in [0.5, 1.5] | 79% |

---

## Verdict

| Claim | Status |
|---|---|
| dens is luminosity density [L⊙/pc²] | Yes (header) |
| dens is **not** inclination-corrected | **Confirmed** (SPARC docs + data) |
| MassModels SBdisk **is** inclination-corrected | **Confirmed** |
| Dominant dens/MM factor is 1/cos i | **Confirmed** (med residual factor 1.01) |
| Exact 1:1 after cos i | Mostly — residual scatter ~25% still present |
| dens recoverable as independent input | **Yes** — apply cos i, then integrate |

The per-galaxy variation of the raw dens/MM ratio is largely the variation of inclination across the sample, not a mysterious galaxy-dependent zero-point.

---

## Practical rule

```text
Σ_for_Vc = dens_SBdisk × cos(i)     # face-on light
# then optional Υ, then Hankel / Casertano
```

Or simply use MassModels SBdisk (already corrected).

After this correction, earlier tests showed V residual falls to ~4% (per-galaxy SB match) or ~10–20% (global factors) — integrator vindicated.

---

## Independence

- dens + published i → **recoverable independent path** (same photometry chain SPARC used before the mass-model step).
- Using MassModels SB directly → validated reimplementation only (circular if claimed as independent V_bar).

Both are useful; they answer different questions.

---

## Remaining scatter (dens×cos i / MM not exactly 1)

Possible: finite thickness in inclination correction, extrapolation differences, kill flags, non-parametric bulge split, numerical interpolation. Secondary to the cos i effect.

# Matched-Υ resolution — the 1.55 is real

Tony Kawas / 11 September 2026.

---

## Three comparisons (disk-only Hankel, same dens SBdisk)

| Comparison | What is compared | med ratio | med rel-err |
|---|---|---|---|
| **A. Υ=1 matched** | \(V_{\mathrm{rec}}(\Sigma=\mathrm{SBd})\) vs \(V_{\mathrm{disk,rotmod}}\) | **1.551** | **62.7%** |
| **B. Υ=0.5 matched** | \(V_{\mathrm{rec}}(\Sigma=0.5\,\mathrm{SBd})\) vs \(V_{\mathrm{disk,rotmod}}\sqrt{0.5}\) | **1.551** | **62.7%** |
| **C. Mismatched (Stage-3 style)** | \(V_{\mathrm{rec}}(\Upsilon=0.5)\) vs \(V_{\mathrm{disk,rotmod}}(\Upsilon=1)\) | **1.097** | **21.4%** |

Identical numbers for A and B (to numerical precision): the ratio is **scale-invariant**. Multiplying both sides by \(\sqrt{0.5}\) cannot change a ratio.

---

## Subsamples (matched, either Υ)

| Sample | med ratio | med rel-err |
|---|---|---|
| All | 1.55 | 62.7% |
| Vfp < 90 | 1.44 | 43.5% |
| Vfp ≥ 90 | 1.60 | 73.6% |
| No dens bulge (N=143) | **1.51** | **54.2%** |
| Has dens bulge (N=32) | 1.62 | 90.5% |

---

## Verdict on the √2 hypothesis

| Claim | Result |
|---|---|
| 1.55 is a Υ-convention mismatch | **Falsified** — matched A and B both give 1.55 |
| Stage-3 “1.51 → 1.06 under Υ=0.5” was the true residual | **Artifact** — that was comparison C (mismatched) |
| Residual is genuine ~55% (ratio 1.55) at matched Υ | **Confirmed** |
| Thickness / Υ bookkeeping can explain it | **No** |

SPARC documents Rotmod at Υ=1. dens is in \(\mathrm{L}_\odot/\mathrm{pc}^2\). At matched Υ the rebuild is systematically high by ~1.55 in velocity (~2.4 in mass).

---

## What Stage 3 actually did

Stage 3 compared a Υ=0.5 prediction to a Υ=1 Rotmod column. That divides the ratio by \(\sqrt{2}\) and produces the comforting ~1.06 / ~20% numbers. Those numbers are **not** a pipeline validation at matched mass-to-light. The honest matched residual remains **~1.55 / ~63%**.

---

## Updated stance

- **Thickness:** still dead.
- **Spherical bulge:** still a real partial fix on the 32 dens-bulge systems (when compared at matched Υ to \(V_\star\)).
- **Dominant residual:** **real**, scale-invariant, present on no-bulge disks → dens↔Rotmod disk construction / extrapolation / zero-point / Hankel on high-SB — not Υ, not thickness.
- **Science:** Rotmod + pre-committed Υ remains the only safe anchor.
- **Home rebuild:** not deployable; matched residual is large.
- **Next (if any):** audit dens vs the exact Σ profile SPARC integrated (outer exponential extrapolation, kill flags, units), or professional external \(V_{\mathrm{bar}}\).

This closes the Υ bookkeeping question. The patient’s chart is now consistent: the large number is real.

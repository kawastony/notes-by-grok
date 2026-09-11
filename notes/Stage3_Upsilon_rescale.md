# Stage 3 follow-up — Υ / normalization check

Tony Kawas / 11 September 2026.

---

## Hypothesis

Prior rebuild used \(\Sigma = 1\times\mathrm{SB}\) (Υ=1). Median \(V_{\mathrm{rec}}/V_{\mathrm{rot}}=1.51\).  
\(\sqrt{2}\approx 1.41\) matches the bulk of that factor if the effective stellar normalization is Υ≈0.5 (pre-committed SPARC convention).

**Note on convention:** SPARC Rotmod columns are published at Υ=1; users scale \(V_{\mathrm{disk}}\) by \(\sqrt{\Upsilon}\). The dens→V mismatch may still be a light-to-mass zero-point / effective-Υ issue in the dens files relative to the mass model that produced Rotmod — empirically testable by rescaling.

---

## Rescale test (175 galaxies, same points as Stage 3)

| Scale on \(V\) | Effective \(\Sigma\) factor | Median rel-err | <10% | <20% | med \(V_{\mathrm{rec}}/V_{\mathrm{rot}}\) |
|---|---|---|---|---|---|
| 1.00 (prior Υ=1) | 1.00 | **58.1%** | 4% | 15% | **1.51** |
| \(\sqrt{0.5}=0.707\) | 0.50 | **20.5%** | 23% | 50% | **1.06** |
| 0.662 (1/1.51) | 0.44 | 21.1% | 18% | 46% | 1.00 |
| **Best 0.700** | **0.49** | **20.5%** | 22% | 48% | 1.05 |

---

## Verdict

| Claim | Status |
|---|---|
| Υ/normalization mismatch is the dominant systematic | **Supported** (1.51 → 1.06) |
| Pipeline matches Rotmod to a few percent after Υ=0.5 | **Not yet** (median residual **~20%**) |
| Thickness / sampling still relevant for residual | **Possible** secondary |
| Ready for external MAE via home rebuild | **Still not** at few-percent level |

The critique was right that Υ was the first thing to check and that thickness alone cannot explain +51%. Fixing Υ removes most of the bias; a ~20% residual remains and must not be papered over.

---

## Pre-commit reminder

For any TAFA MAE (Stage 2 already done): use Rotmod with \(\Upsilon_{\mathrm{disk}}=0.5\), \(\Upsilon_{\mathrm{bul}}=0.7\) — not the home dens rebuild — until residual is closed.

---

## Next

1. Optional: finite-thickness or denser Hankel on high-SB systems to attack the 20% residual.
2. Prefer published professional \(V_{\mathrm{bar}}\) for external samples.
3. Do **not** treat 20% residual rebuild as a theory falsifier or confirmer.

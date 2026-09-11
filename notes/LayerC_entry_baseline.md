# Layer C entry — SPARC baseline reaffirmed

Tony Kawas / 11 September 2026.

After Layer A closure (inclination convention solved; dens only with cos i; science on Rotmod).

---

## Protocol (locked)

- **V_bar:** Rotmod only (not dens rebuild)
- **Υ_disk = 0.5**, **Υ_bul = 0.7** (pre-commit)
- **a_T = 8.25×10^{-11} m s^{-2}** (frozen)
- Interpolator: \(g = \tfrac12 g_N + \sqrt{(\tfrac12 g_N)^2 + g_N a_T}\)
- Metric: per-galaxy median \(|V_{\mathrm{pred}}-V_{\mathrm{obs}}|\) (km/s), points with \(V_{\mathrm{obs}}>10\)

Layer A rules: do not re-open thickness / Υ-mismatch / bulge as causes of the old measuring residual.

---

## Baseline (N=175)

| Model | med MAE (km/s) | mean MAE |
|---|---|---|
| Newton (baryons only) | **38.5** | 41.6 |
| Simple μ + **a_T** | **10.7** | 14.4 |
| Simple μ + a_0 (1.2×10^{-10}) | **10.4** | 14.4 |

| Comparison | Result |
|---|---|
| a_T better than Newton | **161 / 175** galaxies |
| med Newton/a_T | **3.5×** |
| a_T wins vs a_0 | **95 vs 80** |

Consistent with prior scorecard (~10.8 km/s). Layer A work did not change the science anchor.

---

## Layer C open list (from scorecard)

1. **Rate-linearity gap** — motivate → prove interpolator from discrete cone update rule
2. External full V_bar sample (blocked without professional decompositions)
3. Microscopic length without α=1
4. Pause-only observable ≠ ΛCDM
5. Forced high-z a_T (MUSE direction)
6. Cluster Σ_res parameter-free

**Recommended next:** (1) rate-linearity gap — theory, no new data dependency, highest leverage on whether the interpolator is forced or fitted.

---

## Boundary

| Layer | Question |
|---|---|
| A (closed) | Does rebuild match Rotmod? |
| **C (active)** | Does TAFA + locked floor match V_obs? |

Do not import Layer A residuals into Layer C claims.

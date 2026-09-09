# SPARC three follow-ups: deep regime, a0 comparison, BTFR

Tony Kawas / 9 September 2026.
Data: Lelli et al. 2016 (Zenodo 16284118). Υ=0.5, He factor 1.33 on MHI.

Locked floor: \(a_T=8.25\times 10^{-11}\,\mathrm{m\,s^{-2}}\).
Standard MOND scale: \(a_0=1.2\times 10^{-10}\,\mathrm{m\,s^{-2}}\).
Interpolator: simple form \(g=g_N/2+\sqrt{(g_N/2)^2+g_N a}\).

---

## 1. Deep regime (\(g_N < a_T\))

| Quantity | \(a_T\) | \(a_0\) |
|---|---|---|
| Deep points | 2509 | same cut vs \(a_T\) |
| Mean \(\lvert\Delta V\rvert\) | 15.6 km/s | 14.4 km/s |
| Median \(\log_{10}(g_{\mathrm{obs}}/g_{\mathrm{pred}})\) | +0.046 | −0.020 |
| RMS log residual | 0.208 | 0.211 |
| Q=1 galaxies (≥3 deep pts) median MAE | 10.5 km/s | 9.8 km/s |

Deep regime is where the floor should matter most. Both scales work; standard \(a_0\) is slightly tighter on velocity MAE and near-zero median log residual. \(a_T\) sits a bit low (slightly under-predicts acceleration).

---

## 2. Full rotation curves: \(a_T\) vs \(a_0\)

| Sample | N | med MAE \(a_T\) | med MAE \(a_0\) | med MAE Newton |
|---|---|---|---|---|
| Q=1 | 99 | 11.2 | **10.3** | 44.5 |
| Q=2 | 64 | **9.7** | 11.0 | 26.8 |
| All | 175 | **10.8** | 11.9 | 38.2 |

Galaxy wins: \(a_T\) better on **94** galaxies, \(a_0\) on **81**.

Both crush Newtonian baryons-only. Neither dominates the other globally; \(a_0\) wins on high-Q medians, \(a_T\) wins on all-sample median and win count.

---

## 3. Baryonic Tully–Fisher (\(V_{\mathrm{flat}}\) from Table 1)

\[
M_{\mathrm{bar}}=\Upsilon L_{[3.6]}+1.33 M_{\mathrm{HI}},
\qquad \Upsilon=0.5.
\]

Empirical fit (135 galaxies with \(V_{\mathrm{flat}}>0\)):

\[
\log_{10}(M_{\mathrm{bar}}/M_\odot)\approx 3.40 + 3.19\,\log_{10} V_{\mathrm{flat}}
\]

(MOND expectation: slope **4**). Slope is shallower than pure MOND — common with sample cuts and mass systematics.

MOND zero-point test \(M_{\mathrm{pred}}=V^4/(G a)\):

| Sample | median \(\log_{10}(M/M_{\mathrm{pred}})\) \(a_T\) | rms \(a_T\) | median \(a_0\) | rms \(a_0\) |
|---|---|---|---|---|
| All (135) | −0.27 | 0.42 | **−0.10** | **0.36** |
| Q=1 (87) | −0.32 | 0.40 | **−0.16** | **0.29** |

Negative residual: predicted mass above observed (or acceleration scale a bit high relative to this mass convention). Standard \(a_0\) is closer to zero point than \(a_T\).

---

## 4. Compact reading

| Test | Winner |
|---|---|
| Beat Newtonian baryons | **Both** \(a_T\) and \(a_0\) |
| Deep-regime log residual | slight edge **\(a_0\)** |
| Full-curve MAE (all) | slight edge **\(a_T\)** |
| Full-curve MAE (Q=1) | slight edge **\(a_0\)** |
| BTFR zero point | **\(a_0\)** |
| Locked TOE floor integrity | \(a_T\) remains the constitution value |

**Conclusion:** The locked floor is competitive with standard MOND on SPARC under a fixed simple interpolator and Υ=0.5. It is not clearly better. BTFR prefers a slightly larger scale (closer to \(1.2\times 10^{-10}\)). Changing \(a_T\) to match BTFR would be a **calibration choice**, not forced by the DM-floor derivation as written.

---

## 5. Status vs constitution

Keep \(a_T=8.25\times 10^{-11}\) as the locked product unless you deliberately reopen the floor. These tests are evidence for **how far** that number gets you on SPARC, not a mandate to retune it.

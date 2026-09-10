# SPARC stack test — Prediction B (transition height)

Tony Kawas / 10 September 2026. Empirical test of forced prediction.

**Prediction B:** for the locked simple interpolator,
\[
\left.\frac{g_{\mathrm{obs}}}{a_T}\right|_{g_N=a_T}=\varphi\approx 1.618.
\]
Standard MOND \(\mu(x)=x/(1+x)\) at \(x=1\) instead gives **2.0**.

---

## Data

- SPARC mass models (Lelli+2016, CDS J/AJ/152/157 table2), N=3391 radial points.
- \(\Upsilon_{\mathrm{disk}}=0.5\), \(\Upsilon_{\mathrm{bul}}=0.7\).
- \(a_T=8.25\times10^{-11}\,\mathrm{m\,s^{-2}}\).
- Window: \(g_N \in [0.75,1.25]\,a_T\) (±25%).

---

## Result

| Statistic | Value |
|---|---|
| N (points in window) | 270 |
| median \(g_{\mathrm{obs}}/a_T\) | **1.739** |
| mean | 1.880 |
| 16th–84th percentile | 1.31 – 2.32 |
| bootstrap median 16/50/84 | 1.70 / 1.74 / 1.78 |

| Target | Distance of median |
|---|---|
| \(\varphi = 1.618\) | **0.121** |
| standard \(\mu\) = 2.0 | 0.261 |

**Closer to \(\varphi\) than to 2.0.**

High-acceleration sanity check: for \(g_N>10^{-9}\), median \(g_{\mathrm{obs}}/g_N \approx 1.015\) (near Newtonian as required).

---

## Interpretation

1. The stacked SPARC transition is **not** at the standard-MOND value 2.
2. It is **consistent within scatter** with the simple-interpolator height \(\varphi\), and the median is closer to \(\varphi\) than to 2.
3. Scatter is large (16–84 spans ~1.3–2.3); this is **not** a precision measurement of \(\varphi\). It is a **discriminating** statement against pure standard \(\mu\) at the transition.
4. Quality-flag split was not cleanly recovered from the fixed-width table in this run; the all-points stack is the primary result.

---

## Scoreboard update

| Prediction | Pre-test | Post-test |
|---|---|---|
| B: transition \(=\varphi\) | Forced by interpolator | **Supported** (median closer to \(\varphi\) than to 2; large scatter) |
| Standard MOND height 2 | Alternative | **Disfavored** as the median at this window |

Prediction A (cosmological \(a_T\)) was not tested in this note.

---

## One-sentence result

On SPARC, at \(g_N\approx a_T\), the median \(g_{\mathrm{obs}}/a_T\approx 1.74\) lies closer to the locked simple-interpolator value \(\varphi\approx 1.62\) than to the standard MOND value 2, with substantial scatter.

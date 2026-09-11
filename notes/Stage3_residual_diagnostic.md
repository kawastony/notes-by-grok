# Stage 3 residual diagnostic (after Υ=0.5)

Tony Kawas / 11 September 2026.

Wiki check: Observer_Catalyst wiki is slide assets (12.28×, fasting, cone geometry). TAFA-derivation-notes reinforces Forced_vs_Free separation and that 12.28× is not a floor quantity.

---

## Residual vs structure (Υ=0.5 scale on V)

N=175 galaxies.

| Correlation | Value |
|---|---|
| residual ↔ f_bulge | **+0.19** (weak) |
| residual ↔ log median SB | **+0.26** (weak) |
| residual ↔ log max SB | **+0.17** |
| residual ↔ median V_disk | +0.09 |

| Subsample | N | Median residual |
|---|---|---|
| All | 175 | **20.5%** |
| f_bulge ≈ 0 | 145 | 18.6% |
| f_bulge > 0.2 | 20 | 30.0% |
| max SB > 100 | 139 | 21.3% |
| gas-dominated (rough) | 17 | 29.2% |
| star-dominated | 158 | 19.7% |

---

## Categorization

| Hypothesis | Supported? |
|---|---|
| Residual is pure bulge-integration pipeline bug | **Weakly** — mild trend with f_bulge, not dominant |
| Residual is global ~20% floor (input reduction scatter and/or thin-disk vs SPARC mass-model details) | **Better fit** — residual present even at f_bulge≈0 |
| Deployable externally as few-percent instrument | **No** |

Independent professional decompositions often disagree at 10–30%. A 20% residual is compatible with that floor — but that does **not** prove the rebuild is “correct enough” for external use without a reference. It remains **uncategorized enough to park**.

---

## Decision

1. **Science / TAFA MAE:** keep **Rotmod + pre-committed Υ** (Stage 2). That is the live empirical anchor.
2. **Home dens rebuild:** **parked** — development tool only until residual is closed or shown to be pure input-difference with a validated method.
3. **External sample:** still requires professional \(V_{\mathrm{bar}}\) tables or a rebuild that has passed a harder validation than Freeman alone.
4. **Do not** treat 20% residual as evidence for or against TAFA.

Aligned with Forced_vs_Free discipline: do not promote a free/uncertain instrument into a falsifier.

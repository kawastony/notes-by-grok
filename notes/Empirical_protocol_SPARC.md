# Empirical protocol — pre-commit, SPARC run, external status

Tony Kawas / 11 September 2026.

---

## Pre-commit (before results)

| Quantity | Value | Source |
|---|---|---|
| \(\Upsilon_{\mathrm{disk}}\) | **0.5** | SPARC / Lelli convention at 3.6 µm |
| \(\Upsilon_{\mathrm{bul}}\) | **0.7** | SPARC convention |
| \(a_T\) | \(8.25\times10^{-11}\,\mathrm{m\,s^{-2}}\) | Locked calibrated floor |
| Interpolator | simple: \(g=\tfrac12 g_N+\sqrt{(\tfrac12 g_N)^2+g_N a_T}\) | Motivated package (gap on rate linearity accepted) |
| Metric | per-galaxy mean \(|V_{\mathrm{obs}}-V_{\mathrm{model}}\|\) (km/s); report median over galaxies | Fixed |

No post-hoc retuning of \(\Upsilon\) or \(a_T\).

---

## Integrator validation (rebuild path)

Casertano / Bessel thin-disk rebuild from photometry was **not** required for this SPARC run: Rotmod files already supply \(V_{\mathrm{gas}}, V_{\mathrm{disk}}, V_{\mathrm{bul}}\) from the SPARC team’s professional pipeline.

A home-built integrator is only needed for true external rebuild from HI cubes + Spitzer when published radial baryonic splits are unavailable. That validation (Freeman exponential disk to ≲1%) remains **mandatory before any cube-based external sample**, and is deferred — not skipped as a permanent exemption.

---

## SPARC result (this run)

Data: `Rotmod_LTG.zip` (175 galaxies, 3391 points).

| Model | Median per-galaxy MAE (km/s) | Mean per-galaxy MAE |
|---|---|---|
| Newtonian (\(g=g_N\)) | **37.41** | 39.93 |
| TAFA simple + frozen \(a_T\) | **10.82** | 14.91 |
| Improvement | **3.46×** | — |

Consistent with prior SPARC scorecard entries (~10.8 vs ~38).

---

## External transfer status

| Source | Status |
|---|---|
| Oh+2015 CDS `rotdmbar` | Total \(V\) only — no radial \(V_{\mathrm{gas}}, V_\star\) |
| de Blok+2008 THINGS | Not yet pulled with full decomposition in this session |
| Cube rebuild | Open, expensive; needs validated integrator + pre-committed \(\Upsilon\) |

Empirical door for a **true** external MAE test remains open but not completed.

---

## Discipline checklist

- [x] Pre-commit \(\Upsilon\) and \(a_T\)
- [x] SPARC run under freeze
- [ ] Freeman validation of home integrator (before cube rebuild)
- [ ] External sample with full \(V_{\mathrm{bar}}(r)\)

---

## One line

Under pre-committed SPARC \(\Upsilon\) and locked \(a_T\), simple interpolator delivers median ~10.8 km/s vs Newtonian ~37 on all 175 SPARC galaxies; external generalization still pending machine-readable radial baryonic splits or a validated rebuild pipeline.

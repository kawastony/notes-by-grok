# Open B — compute ε_cone from TAFA 5D warp

Tony Kawas / 12 September 2026. High-value step after Layer C reconciliation.

---

## Setup (from old Open B / Paper 38 action)

\[
A''=-\frac13(\phi')^2,\qquad
\phi''+4A'\phi'=V_A'(\phi),\qquad
V_A=\Lambda^4\tan^2(\phi/2f).
\]

Unit chart: \(f=\Lambda=1\). Domain \(|\phi|<\pi\). No \(11/72\) in any loss function.

Constraint monitor: \(V=\tfrac12(\phi')^2-6(A')^2\).

Anisotropy measure from stress tensor: \(T_{yy}-(-(\tfrac12\phi'^2+V))\sim \phi'^2\).

Warped residual fractions:
\[
\varepsilon^{(2)}=\frac{\int\phi'^2 e^{2A}\,\mathrm{d}y}{\int(\tfrac12\phi'^2+V)e^{2A}\,\mathrm{d}y},\qquad
\varepsilon^{(4)}=\frac{\int\phi'^2 e^{4A}\,\mathrm{d}y}{\int(\tfrac12\phi'^2+V)e^{4A}\,\mathrm{d}y}.
\]

---

## Numerical results (N=30 nontrivial starts)

| Quantity | Median | p16–p84 |
|---|---|---|
| \(\varepsilon^{(2)}\) | **1.34** | 1.26–1.39 |
| \(\varepsilon^{(4)}\) | **1.31** | 1.23–1.37 |
| \(A_{\mathrm{end}}\) | **−0.44** | (old wall target \(A\to-1/2\)) |
| \(|A'_{\mathrm{end}}|\) | **1.45** | — |
| Runs with \(|A'|\approx 11/72\) | **0** | — |

---

## What this measures

### Confirmed (old Open B)

- **\(11/72\) is not an eigenvalue** of the consistent TAFA 5D system under regular/near-tip data.
- \(A'\) is non-increasing from \(A'(0)=0\) and grows to **O(1)**, not to \(11/72\).
- Wall behaviour: \(A\to\sim-1/2\) matches the old wall target in the unit chart.

### Residual magnitude in unit chart

\[
\varepsilon_{\mathrm{cone}}^{\mathrm{(unit)}}\;=\;\mathcal{O}(1)
\]

The anisotropic piece is **comparable to** the local energy density in the unit chart — not a small parameter. So:

- One **cannot** treat \(\varepsilon_{\mathrm{cone}}\) as a tiny perturbation that automatically yields \(|\eta|\sim0.05\)–0.15 in 4D.
- A controlled 4D slip amplitude requires a **further reduction step**: how this O(1) 5D anisotropy projects onto 4D cosmological variables after matching to the observed Planck scale, freeze density, and warped volume. That step is still Open.

### What is **not** claimed

| Claim | Status |
|---|---|
| \(\varepsilon_{\mathrm{cone}}=11/72\) | **False** as 5D output |
| Unit-chart \(\varepsilon\sim1\) ⇒ 4D \(|\eta|\sim1\) | **Not justified** — reduction map missing |
| Unit-chart \(\varepsilon\sim1\) ⇒ 4D \(|\eta|\sim0\) | **Not justified** either |
| Homogeneous pause sources slip | Still **false** (old \(T_{\mu\nu}\)) |

---

## Status of the outward discriminator

| Piece | Status after this computation |
|---|---|
| Channel | Warp anisotropic residual — **confirmed present at O(1) in unit chart** |
| Timing | \(z\sim0.3\) activation interval — **unchanged, derived** |
| 4D amplitude \(|\eta|\) | **Still not computed** — needs 5D→4D projection map |
| Direct \(11/72\to\|\eta\|\) | **Remains retracted** |

**Plain language:** the funnel **does** carry O(1) anisotropic stress in the unit chart, and it is **not** tuned to 11/72. Whether 4D observers see a percent-level slip or a negligible one depends on a reduction that is not yet done.

---

## Next (if pursued)

1. **4D projection map:** reduce the computed 5D \(T_{MN}\) on the warped background to effective 4D anisotropic stress \(\Sigma\) or \(\sigma\) at the freeze epoch (match \(M_{\mathrm{Pl}}\), \(\rho_\Lambda\), volume).  
2. **Or stop** and keep the discriminator as mechanism + clock without amplitude.

Do **not** re-insert 11/72 as a 5D target. Do **not** reopen SPARC form derivation.

---

## One-sentence close

Open B on the TAFA potential confirms anisotropic warp residual of **order unity in the unit chart** and **rejects** 11/72 as a 5D slope eigenvalue; the quantitative 4D slip amplitude remains open until the warped stress is projected onto cosmological variables, so TAFA still has a clock and a channel, not yet a measured η.

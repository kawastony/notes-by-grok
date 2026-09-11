# Constitutive map attack — residual strain → slip

Tony Kawas / 11 September 2026. Layer C.

Goal: bound or derive the order-unity factor that converts locked residual
\((11/72)_{\mathrm{cone}}\approx0.15\) into observable late-time gravitational slip
\(|\eta|=|\Phi/\Psi-1|\).

---

## 1. What must be mapped

\[
\varepsilon_{\mathrm{res}}\;\sim\;\frac{11}{72}
\qquad\longrightarrow\qquad
|\eta|_{z\,\lesssim\,0.3}\;=\;\alpha_{\mathrm{c}}\,\varepsilon_{\mathrm{res}}
\]

\(\alpha_{\mathrm{c}}\) is the constitutive factor. Previously: unknown \(\mathcal{O}(1)\).

---

## 2. Volume constraint forces the residual into the traceless channel

Locked volume constraint (cone / waist):
\[
R^2 L = \mathrm{Vol}_0\quad\Rightarrow\quad
N\bigl(2 L A_\phi\, p + 1\bigr)=0.
\]

**Pause branch:** \(N=0\), field frozen.

**Geometry of residual:** any incomplete freeze of a **volume-preserving** deformation leaves a residual **shape** mismatch, not a residual **volume** mismatch.

In continuum language, volume-preserving strain is **traceless**:
\[
\mathrm{tr}\,\varepsilon_{\mathrm{res}} = 0.
\]

**Consequence:**

| Channel | Trace residual | Traceless residual |
|---|---|---|
| Renormalizes effective \(\Lambda\) | Yes | No |
| Sources anisotropic stress \(\sigma\) | No | **Yes** |
| Sources gravitational slip \(\eta\) | No | **Yes** |

A pure potential freeze (isotropic residual density) would give \(\sigma=0\) and \(\eta=0\) — constitutive factor → 0, prediction dies.

Volume preservation **forbids** dumping the residual entirely into the trace. The residual is forced into the **anisotropic stress channel**. That is the structural content of the constitutive map.

---

## 3. Amplitude bounds on \(\alpha_{\mathrm{c}}\)

### Upper bound (all residual anisotropic)

If the entire bookkeeping residual is available as anisotropic stress relative to the freeze density:
\[
\alpha_{\mathrm{c}}^{\mathrm{(max)}}\;\sim\;1
\qquad\Rightarrow\qquad
|\eta|\;\lesssim\;\frac{11}{72}\approx0.15
\]
at late times when DE is dynamically important and the quasi-static slip responds to that stress.

### Orientation average (network of cones)

Local cone elongation has a preferred axis. Cosmological residual is an average over orientations.

For randomly oriented traceless dipoles / uniaxial residuals in 3D, the sky-averaged anisotropic stress is suppressed by a geometric factor of order
\[
\frac{1}{3}\quad\text{to}\quad\frac{2}{5}
\]
(typical of averaging \(P_2(\cos\theta)\) or stress-tensor projections).

Take
\[
\alpha_{\mathrm{c}}^{\mathrm{(avg)}}\;\sim\;\frac{1}{3}
\qquad\Rightarrow\qquad
|\eta|\;\sim\;\frac{11}{72}\times\frac{1}{3}\;\approx\;0.05.
\]

### Lower bound (not zero)

Volume preservation blocks \(\alpha_{\mathrm{c}}\to0\). A conspiracy that restores full isotropy after orientation average would require the residual network to be tuned to a pure trace — forbidden by the same constraint that defines the residual.

**Working interval:**
\[
\boxed{0.05\;\lesssim\;|\eta|_{z\,\lesssim\,0.3}\;\lesssim\;0.15}
\]
i.e. \(\alpha_{\mathrm{c}}\in[\sim1/3,\,1]\), not a free parameter of either extreme.

---

## 4. Relation to linearized GR (honest)

In the Newtonian gauge, anisotropic stress sources
\[
\Phi-\Psi \;\propto\; a^2(\rho+P)\sigma\,/\,k^2
\]
(scheme-dependent factors). At late times, on sub-horizon scales relevant to weak lensing / \(E_G\), the mapping from a relative stress \(\delta P_{\mathrm{aniso}}/\rho_\Lambda\sim\varepsilon_{\mathrm{res}}\) to \(\eta\) is **order unity** when DE dominates the background budget that multiplies \(\sigma\). That is why \(\alpha_{\mathrm{c}}\sim\mathcal{O}(1)\) is the natural quasi-static reading — not an extra assumption beyond “residual stress is a fraction \(\varepsilon_{\mathrm{res}}\) of the freeze density.”

A full Boltzmann or scalar-tensor calculation would replace the interval with a function of \(k\) and \(z\). Until that exists, the interval above is the **structural bound**, not a fit.

---

## 5. Re-confrontation with \(\Sigma_0\)

Published (smooth late MG, DESI+CMB+DES-Y3):
\[
\Sigma_0 = 0.008\pm0.045\quad(1\sigma).
\]

| Assumed \(\alpha_{\mathrm{c}}\) | Predicted \(|\eta|\) | vs \(\Sigma_0\) width |
|---|---|---|
| 1 | ~0.15 | ~3σ tension if 1:1 with \(\Sigma\) |
| 1/3 | ~0.05 | ~1σ — marginal, allowed |
| ≪1/3 | ≪0.05 | comfortable — **disfavored by volume-preserving argument** |

**Updated status:**

- Naive full mapping (\(\alpha_{\mathrm{c}}=1\)) is under **real pressure** from smooth-template \(\Sigma_0\).
- Orientation-averaged mapping (\(\alpha_{\mathrm{c}}\sim1/3\)) sits at the edge of current sensitivity.
- The volume-preserving argument **forbids** retreating to arbitrarily small \(\alpha_{\mathrm{c}}\) to evade bounds.

Still not a direct kill: templates are smooth \(\Omega_{\mathrm{DE}}\) evolution, not a step at \(z\sim0.3\).

---

## 6. What is forced vs soft after this attack

| Item | Status |
|---|---|
| Residual size \(11/72\) | Locked accounting |
| Residual is traceless (volume-preserving) | **Forced** by cone constraint |
| Residual sources anisotropic stress, not only \(\Lambda\) | **Forced** |
| \(\alpha_{\mathrm{c}}\) cannot be ≪1 | **Forced** (order-unity lower bound ~1/3) |
| Exact \(\alpha_{\mathrm{c}}=1\) vs \(1/3\) | Soft — orientation average |
| Full \(k,z\)-dependent transport | Open |
| Step vs smooth template mismatch | Still limits direct exclusion |

---

## 7. Filed prediction (updated)

\[
|\eta|_{z\,\lesssim\,0.3}\;\in\;[0.05,\,0.15]
\]
with turn-on near the activation interval, at fixed ΛCDM expansion history.

GR and Simple-μ MOND+Λ: \(\eta=0\).

---

## 8. Do not claim

- That \(\alpha_{\mathrm{c}}\) is computed from a varied action to three digits.
- That \(\Sigma_0\) already excludes the model (template mismatch).
- That the map is closed with zero soft joints.

---

## One-sentence close

Volume preservation forces the freeze residual into **traceless** stress, so the constitutive factor cannot collapse to zero; the observable late-time slip is bounded to **\(|\eta|\in[0.05,0.15]\)** for \(z\lesssim0.3\), putting the upper edge under pressure from current \(\Sigma_0\) and the lower edge at the margin of detectability — the soft joint is narrowed from “any \(\mathcal{O}(1)\)” to a definite interval with a structural floor.

# B — Action-level 5D	o4D reduction (η last)

Tony Kawas / 12 September 2026. Zero-knobs protocol.

---

## 0. Inputs (locked, no tuning)

**5D action** (Paper 38 / Open B, units \(M_5^3=1\)):
\[
S_5=\int\mathrm{d}^5x\,\sqrt{-G}\left[
\tfrac12 R_5
-\tfrac12 G^{MN}\partial_M\phi\,\partial_N\phi
-V(\phi)
\right],
\qquad
V=V_A=\Lambda^4\tan^2(\phi/2f).
\]

**Metric ansatz** (warped product, vacuum slices):
\[
\mathrm{d}s_5^2
=e^{2A(y)}\,\eta_{\mu\nu}\,\mathrm{d}x^\mu\mathrm{d}x^\nu
+\mathrm{d}y^2,
\qquad
\phi=\phi(y)\ \text{only}.
\]

**Euler–Lagrange / Einstein equations** (already derived):
\[
A''=-\tfrac13(\phi')^2,
\qquad
6(A')^2=\tfrac12(\phi')^2-V,
\qquad
\phi''+4A'\phi'=V'(\phi).
\]

No \(11/72\) target. No observational window until the end.

---

## 1. 5D stress tensor (exact)

\[
T_{\mu\nu}
=-e^{2A}\bigl(\tfrac12(\phi')^2+V\bigr)\,\eta_{\mu\nu},
\qquad
T_{yy}
=\tfrac12(\phi')^2-V.
\]

**Structural fact:**
\[
T_{\mu\nu}\ \propto\ \eta_{\mu\nu}.
\]
On every fixed-\(y\) 4D slice the bulk stress is a **perfect fluid**: isotropic pressure, no preferred spatial direction in the three large dimensions.

Define the spatial anisotropic stress (what sources gravitational slip):
\[
\Pi_{ij}
=T_{ij}-\tfrac13\delta_{ij}\delta^{kl}T_{kl}
\quad\text{(traceless spatial)}.
\]
For \(T_{\mu\nu}\propto\eta_{\mu\nu}\):
\[
\boxed{\Pi_{ij}=0}.
\]

---

## 2. Dimensional reduction to effective 4D stress

Einstein-frame 4D Planck mass:
\[
M_{\mathrm{Pl}}^2
=\int\mathrm{d}y\,e^{2A(y)}
\quad(M_5^3=1).
\]

Effective 4D energy density from the bulk (standard warped integral):
\[
\rho_{\mathrm{eff}}
\propto
\frac{1}{M_{\mathrm{Pl}}^2}
\int\mathrm{d}y\,e^{2A}\bigl(\tfrac12(\phi')^2+V\bigr).
\]
Effective 4D isotropic pressure is fixed by the same integral structure (perfect-fluid reduction of a perfect-fluid bulk). The **yy-versus-μν** bulk anisotropy is absorbed into the overall amplitude of \(\rho_{\mathrm{eff}}\) (and any residual cosmological-term correction); it does **not** generate a traceless spatial \(\Pi_{ij}\) on the 4D slices.

Therefore:
\[
T^{(4)}_{\mu\nu}
=(\rho_{\mathrm{eff}}+p_{\mathrm{eff}})u_\mu u_\nu+p_{\mathrm{eff}}g_{\mu\nu}
+\underbrace{0}_{\Pi_{\mu\nu}}.
\]

---

## 3. Gravitational slip — read last

In Newtonian gauge, spatial anisotropic stress sources
\[
\Phi-\Psi\ \propto\ \Pi.
\]
With \(\Pi_{ij}=0\):
\[
\boxed{\eta\equiv\Phi/\Psi-1\ =\ 0}
\]
from the homogeneous, \(y\)-only bulk sector of this action and ansatz.

This is the action-forced amplitude for **this** reduction class. No free factor was inserted.

---

## 4. What the earlier \(\varepsilon\sim\mathcal{O}(1)\) actually was

The unit-chart residual
\[
\varepsilon
=\frac{\int\phi'^2 e^{2A}\,\mathrm{d}y}{\int(\tfrac12\phi'^2+V)e^{2A}\,\mathrm{d}y}\sim 1.3
\]
measures **bulk** anisotropy between the extra dimension and the 4D directions (\(T_{yy}\) vs \(T_{\mu\nu}\)).

That is a real geometric residual. Under the correct reduction it corrects **effective density / warp pressure**, not 4D **slip**.

Mapping that number directly onto \(|\eta|\) was a **category error** (5D bulk anisotropy \(\neq\) 4D spatial \(\Pi_{ij}\)). The pre-registered “failure high” was a failure of that map, not a proof that the action predicts large slip.

---

## 5. When could \(\eta\neq 0\) still appear?

Only with **extra** structure beyond the locked homogeneous ansatz:

| Source of \(\Pi_{ij}\neq 0\) | In current B? |
|---|---|
| \(y\)-only homogeneous scalar | **No** |
| \(x\)-dependent bulk perturbations | Not in ansatz |
| Brane-localized anisotropic matter | Not in action |
| Vector/tensor bulk modes | Not excited here |
| Explicit 4D isotropy breaking | Not present |

So B does not claim “slip is impossible in all of TAFA.” It claims: **the homogeneous warp + TAFA scalar sector of the Paper 38 action produces zero 4D gravitational slip.**

---

## 6. Consistency with the freeze

| Item | Status after B |
|---|---|
| Quantitative \(|\eta|\sim 0.05\)–0.15 from unit-chart \(\varepsilon\) | **Still dead** (wrong anisotropy) |
| Homogeneous pause / bulk \(\Rightarrow\) large slip | **False** — action says \(\eta=0\) |
| Warp residual as density/warp-pressure correction | **Alive** (\(\varepsilon\sim\mathcal{O}(1)\) unit chart) |
| Clock \(z\sim 0.3\) | **Unchanged** |
| Need new structure for nonzero slip | Yes — and it must be derived, not inserted |

B **strengthens** the freeze: the tested homogeneous reduction does not overpredict slip; it predicts **none**. The earlier overprediction was an incorrect identification of which stress component sources \(\Phi-\Psi\).

---

## 7. One-sentence close

Varying the locked Paper 38 action on a warped product with a \(y\)-only TAFA scalar yields a 4D effective stress that is a perfect fluid (\(\Pi_{ij}=0\)), so gravitational slip is **zero** from this sector; the previously computed \(\mathcal{O}(1)\) residual is bulk yy–μν anisotropy that corrects density, not 4D slip, and any nonzero \(\eta\) requires additional derived structure beyond this ansatz.

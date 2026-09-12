# Linear anisotropic stress around the locked background

Tony Kawas / 12 September 2026. Forced perturbation derivation — η last.

---

## 0. Background (locked)

\[
ds_5^2 = e^{2A(y)}\bar g_{\mu\nu}(t)\,dx^\mu dx^\nu + dy^2,
\qquad
\phi_0=\phi_0(y),
\qquad
\partial_i\phi_0=0,\ \phi_0'\neq0.
\]
\[
T^{(0)}_{\mu\nu}\propto g^{(0)}_{\mu\nu},
\qquad
\eta^{(0)}=0,
\qquad
w_{\mathrm{eff}}^{(0)}=-1.
\]

---

## 1. Perturbations

\[
\phi=\phi_0(y)+\delta\phi(x^\mu,y),
\qquad
g_{MN}=g^{(0)}_{MN}+h_{MN}.
\]
Retain \(h_{\mu y}\) until shown nondynamical.

Scalar stress (canonical):
\[
T_{MN}=\partial_M\phi\,\partial_N\phi
-g_{MN}\bigl(\tfrac12(\partial\phi)^2+V\bigr).
\]

---

## 2. Linear mixed component (gate)

\[
\delta T_{\mu y}\big|_{\mathrm{scalar}}
=\phi_0'\,\partial_\mu\delta\phi
+\text{(metric perturbation pieces)}.
\]

Einstein: \(\delta G_{\mu y}=\kappa_5^2\delta T_{\mu y}\).

With \(h_{\mu y}=0\) (or pure gauge), the scalar piece requires
\[
\phi_0'\,\partial_\mu\delta\phi
\)
to be cancelled by the linearized curvature or to vanish. This constrains the admissible \(\delta\phi\) (radion-like / constrained scalar), rather than allowing free 4D-dependent bulk scalars with unconstrained spatial gradients.

**Gate result:** 4D-dependent \(\delta\phi\) is not free; it is tied to the mixed constraint and metric sector.

---

## 3. Linear traceless spatial stress from the scalar

\[
\delta T_{ij}\big|_{\mathrm{scalar,\ gradients}}
=\partial_i\delta\phi\,\partial_j\phi_0
+\partial_i\phi_0\,\partial_j\delta\phi
+\cdots
\]

But \(\partial_i\phi_0=0\), so the **gradient–gradient anisotropic structure vanishes at linear order**:
\[
\partial_i\delta\phi\,\partial_j\phi_0=0.
\]

Remaining scalar contributions to \(\delta T_{ij}\) at linear order are of the form
\[
-\delta g_{ij}\,\mathcal L_0
-g^{(0)}_{ij}\,\delta\mathcal L,
\]
i.e. **isotropic** (pure trace). They renormalize effective density and pressure perturbations; they do not build a traceless spatial \(\Pi_{ij}\).

**Scalar-sector theorem (linear):**
\[
\boxed{\Pi_{ij}^{(\mathrm{scalar,\ linear})}=0}.
\]

Therefore the TAFA scalar does **not** source gravitational slip at linear order around this background.

---

## 4. Gauge-invariant reading

In 4D language, after reduction,
\[
k^2(\Phi-\Psi)\propto a^2\Pi_{\mathrm{eff}}.
\]
With \(\Pi_{\mathrm{eff}}^{(\mathrm{scalar,\ linear})}=0\),
\[
\Phi=\Psi
\]
at linear order from the scalar sector alone (up to residual gauge / constraint modes that do not invent new shear).

---

## 5. What this does **not** close

| Sector | Status |
|---|---|
| Linear TAFA scalar \(\Pi_{ij}\) | **Vanishes** |
| Bulk **graviton / Weyl** anisotropic stress (5D gravity KK) | Not computed; known in braneworld literature to be possible in principle |
| Nonlinear scalar stress \(\partial_i\delta\phi\,\partial_j\delta\phi\) | Second order; not a linear slip source |
| Brane-localized matter shear | Not in the bulk scalar action |

The Paper 38 action includes 5D Einstein gravity, so bulk metric perturbations are not absent. A full proof that **all** linear slip vanishes would require showing the projected Weyl / KK contribution is zero or negligible after reduction — that is a separate calculation, not claimed here.

**Claim filed:** the **TAFA scalar sector** does not generate linear slip on this background. Any residual linear slip would have to come from **bulk gravity modes**, not from the scalar residual that drove the earlier amplitude saga.

---

## 6. Relation to the amplitude autopsy

| Attempt | Verdict |
|---|---|
| Background \(11/72\to\eta\) | Dead |
| Unit-chart \(\varepsilon\to\eta\) | Category error (bulk yy vs 4D shear) |
| Homogeneous sector | \(\eta=0\) theorem |
| Linear scalar perturbations | \(\Pi_{ij}=0\) — no slip from scalar |

The scalar channel is closed at linear order for the same structural reason the background was closed: **no spatial gradients in the background field** to seed linear anisotropic stress.

---

## 7. One-sentence close

Linearizing the TAFA scalar on the locked \(\phi_0(y)\) background yields vanishing traceless spatial stress at first order because \(\partial_i\phi_0=0\), so the scalar sector does not source slip; residual linear slip, if any, would have to come from bulk graviton/Weyl modes, which are not computed here and are not the scalar residual pursued in the amplitude sequence.

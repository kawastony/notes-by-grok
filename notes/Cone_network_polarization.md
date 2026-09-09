# Polarization vectors on the cone network

Tony Kawas / 9 September 2026. Derivation note. Builds on `Cone_network_transfer.md`.

Laws 1–3 unchanged. Law 4: source = deformation of the cone medium. Boundary = allowed values of that deformation.

---

## 1. Why a scalar is not enough

Scalar elongation \(\varepsilon\) has one degree of freedom per site. A free photon has **two** helicities. Promote the site variable to a spatial vector (deformation of the local cone frame):

\[
\boldsymbol{\varepsilon}_i(t)\in\mathbb{R}^3.
\]

Continuum field: \(\boldsymbol{\varepsilon}(\mathbf{x},t)\).

---

## 2. Action (linear, quadratic floor)

\[
S=\int\mathrm{d}t\,\mathrm{d}^3x\,\frac{\mu}{2}\Big[
(\partial_t\boldsymbol{\varepsilon})^2
- c^2(\partial_i\varepsilon_j)(\partial_i\varepsilon_j)
- \omega_0^2\boldsymbol{\varepsilon}^2
\Big]
\]

with the same emergent speed as the scalar network:

\[
c^2=\frac{\kappa a^2}{\mu}.
\]

Euler–Lagrange:

\[
\partial_t^2\boldsymbol{\varepsilon} - c^2\nabla^2\boldsymbol{\varepsilon} + \omega_0^2\boldsymbol{\varepsilon}=0.
\]

This still has **three** components. A photon-like mode needs a constraint that removes the longitudinal piece.

---

## 3. Constraint: volume / no local compression along the ray

Stadium-wave picture: the pattern is a **shape change handed sideways**, not a bulk pile-up along the direction of travel.

Impose the continuum constraint (Law 3 style: closes the interaction)

\[
\nabla\cdot\boldsymbol{\varepsilon}=0
\qquad\text{(transverse deformations only).}
\]

Equivalent statement for a plane wave \(e^{i(\mathbf{k}\cdot\mathbf{x}-\omega t)}\):

\[
\mathbf{k}\cdot\boldsymbol{\varepsilon}=0.
\]

If the cone volume form is written with a local radial frame, the same condition is the linearised “no net radial compression of the packet along \(\hat k\).”

(Optional stronger cone wall: \(\lvert\boldsymbol{\varepsilon}\rvert\le\varepsilon_{\max}\). Not needed for the polarization basis.)

---

## 4. Plane-wave sector

Set \(\omega_0=0\) for the transfer channel (gapless hand-off). Dispersion:

\[
\omega^2 = c^2\lvert\mathbf{k}\rvert^2
\qquad\Rightarrow\qquad
\omega = c\lvert\mathbf{k}\rvert
\]

(positive frequency). Direction of propagation:

\[
\hat{\mathbf{k}}=\frac{\mathbf{k}}{\lvert\mathbf{k}\rvert}.
\]

The amplitude is a constant vector \(\mathbf{e}\) with

\[
\mathbf{e}\cdot\hat{\mathbf{k}}=0,
\qquad
\lvert\mathbf{e}\rvert=1
\]

(for linear polarization of unit strength).

---

## 5. Derivation of two polarization vectors

The plane orthogonal to \(\hat{\mathbf{k}}\) is two-dimensional. Choose any right-handed orthonormal triad

\[
(\hat{\mathbf{k}},\,\mathbf{e}^{(1)},\,\mathbf{e}^{(2)}).
\]

**Construction (explicit)**

1. Pick a fixed reference axis not parallel to \(\hat{\mathbf{k}}\), e.g. \(\hat{\mathbf{z}}\), unless \(\hat{\mathbf{k}}\parallel\hat{\mathbf{z}}\) then use \(\hat{\mathbf{x}}\).
2. Set

\[
\mathbf{e}^{(1)}
=
\frac{\hat{\mathbf{z}}\times\hat{\mathbf{k}}}{\lvert\hat{\mathbf{z}}\times\hat{\mathbf{k}}\rvert}.
\]

3. Set

\[
\mathbf{e}^{(2)}
=
\hat{\mathbf{k}}\times\mathbf{e}^{(1)}.
\]

Then, by algebra of the cross product:

\[
\mathbf{e}^{(1)}\cdot\hat{\mathbf{k}}=0,
\qquad
\mathbf{e}^{(2)}\cdot\hat{\mathbf{k}}=0,
\]

\[
\mathbf{e}^{(1)}\cdot\mathbf{e}^{(2)}=0,
\qquad
\lvert\mathbf{e}^{(1)}\rvert=\lvert\mathbf{e}^{(2)}\rvert=1,
\]

\[
\mathbf{e}^{(1)}\times\mathbf{e}^{(2)}=\hat{\mathbf{k}}.
\]

These are the **two linear polarization vectors** for propagation direction \(\hat{\mathbf{k}}\).

---

## 6. Completeness in the transverse plane

Any transverse amplitude decomposes uniquely:

\[
\mathbf{e}
=
\sum_{\lambda=1}^{2}
(\mathbf{e}\cdot\mathbf{e}^{(\lambda)})\,\mathbf{e}^{(\lambda)},
\qquad
\mathbf{e}\cdot\hat{\mathbf{k}}=0.
\]

Projector onto physical polarizations:

\[
P_{ij}
=
\delta_{ij}-\hat{k}_i\hat{k}_j
=
\sum_{\lambda=1}^{2}e^{(\lambda)}_i e^{(\lambda)}_j.
\]

That is the completeness relation for the two polarization vectors.

---

## 7. Circular (helicity) basis

Define

\[
\mathbf{e}^{(\pm)}
=
\frac{1}{\sqrt{2}}\big(\mathbf{e}^{(1)}\pm i\mathbf{e}^{(2)}\big).
\]

Then

\[
\hat{\mathbf{k}}\cdot\mathbf{e}^{(\pm)}=0,
\qquad
(\mathbf{e}^{(\pm)})^*\cdot\mathbf{e}^{(\pm)}=1,
\qquad
(\mathbf{e}^{(\pm)})^*\cdot\mathbf{e}^{(\mp)}=0.
\]

Under a rotation by \(\psi\) about \(\hat{\mathbf{k}}\),

\[
\mathbf{e}^{(\pm)}\mapsto e^{\mp i\psi}\mathbf{e}^{(\pm)},
\]

so helicity \(\pm 1\). Same two degrees of freedom, different basis.

---

## 8. General transverse packet on the network

\[
\boldsymbol{\varepsilon}(\mathbf{x},t)
=
\sum_{\lambda=1}^{2}
\int\frac{\mathrm{d}^3k}{(2\pi)^3}\,
\Big[
\mathbf{e}^{(\lambda)}(\hat{\mathbf{k}})\,a_{\mathbf{k}\lambda}\,e^{i(\mathbf{k}\cdot\mathbf{x}-c\lvert\mathbf{k}\rvert t)}
+
\mathrm{c.c.}
\Big].
\]

Only \(\lambda=1,2\) appear. The longitudinal direction is absent by the constraint \(\mathbf{k}\cdot\boldsymbol{\varepsilon}=0\).

---

## 9. What is derived vs open

| Object | Status |
|---|---|
| Vector elongation on the cone lattice | Defined |
| Transversality \(\mathbf{k}\cdot\mathbf{e}=0\) from no longitudinal compression | Imposed (geometric constraint) |
| Two orthonormal \(\mathbf{e}^{(1)},\mathbf{e}^{(2)}\) for each \(\hat{\mathbf{k}}\) | **Derived** by cross-product construction |
| Helicity basis \(\mathbf{e}^{(\pm)}\) | **Derived** from the linear pair |
| Completeness \(P_{ij}=\delta_{ij}-\hat k_i\hat k_j\) | **Derived** |
| Maxwell field strength, gauge field \(A_\mu\), spin-1 representation of Lorentz group | **Not derived** — this is still a constrained vector wave on the network |
| Why the constraint is forced by the TAFA wall (not only imposed) | Open |

---

## 10. Compact statement

For each propagation direction \(\hat{\mathbf{k}}\) on the cone network, the allowed polarization vectors are the orthonormal basis of the plane perpendicular to \(\hat{\mathbf{k}}\):

\[
\mathbf{e}^{(1)}=\frac{\hat{\mathbf{z}}\times\hat{\mathbf{k}}}{\lvert\hat{\mathbf{z}}\times\hat{\mathbf{k}}\rvert},
\qquad
\mathbf{e}^{(2)}=\hat{\mathbf{k}}\times\mathbf{e}^{(1)},
\]

with circular combinations \(\mathbf{e}^{(\pm)}=(\mathbf{e}^{(1)}\pm i\mathbf{e}^{(2)})/\sqrt{2}\).

That is the polarization structure of the gapless transverse elongation wave. It is the minimum vector upgrade of the stadium-wave cone network.

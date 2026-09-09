# Topological charge on the cone network (link to TAFA / TIFA)

Tony Kawas / 9 September 2026. Derivation sketch. Connects defects to old TAFA field space.

Energy minimisation gave \(\chi_c=0\). Topology is the remaining lever that can force a **nonzero integer** without minimising a free amplitude.

---

## 1. What topology can and cannot do here

A topological charge is the degree (or winding) of a map from a surface around the defect into a **compact** target manifold. Continuous deformation cannot change the integer if the target stays compact and the map stays continuous.

| Target | Relevant homotopy | Typical defect |
|---|---|---|
| \(S^1\) (circle) | \(\pi_1(S^1)=\mathbb{Z}\) | vortex / flux line (loop around defect) |
| \(S^2\) | \(\pi_2(S^2)=\mathbb{Z}\) | point hedgehog / monopole-like core |
| Interval with walls (TAFA) | not a closed manifold | **no** integer from pure topology until ends are identified or infinity is compactified |

So: plain TAFA \(\lvert\phi\rvert<\pi f\) as an open interval does **not** by itself give \(\pi_2\) integers. We need a circle, a sphere, or a compactification that old TAFA already almost has.

---

## 2. Route TIFA — circle from the periodic parent

TIFA: \(V_T=\Lambda^4(1-\cos\phi/f)\). Field is **periodic** with period \(2\pi f\). Target is a circle \(S^1\) of radius related to \(f\).

Around a **line** defect (or a vacancy viewed in a plane perpendicular to a preferred axis),

\[
\oint_{S^1} \mathrm{d}\phi = 2\pi f\, n,
\qquad n\in\mathbb{Z}.
\]

Winding \(n\) is the integer. Continuous dynamics that never leave the TIFA circle cannot change \(n\).

**EM reading on the network**

- Natural for **magnetic flux** / Aharonov–Bohm phase: \(\oint\mathbf{A}\cdot\mathrm{d}\boldsymbol{\ell}\propto n\).
- Matches Model C (dislocation / Burgers) more than static electric monopole.
- Old golden-bridge identity TIFA\(\leftrightarrow\)TAFA still maps the circle to a walled interval; the integer lives most cleanly on the **TIFA** side.

**Status:** integer exists; it is vortex-like, not yet Coulomb \(q\).

---

## 3. Route TAFA walls — compactify by the pole

TAFA: \(V_A=\Lambda^4\tan^2(\phi/2f)\), walls at \(\phi=\pm\pi f\). Potential \(\to\infty\) at both ends.

**Compactification:** identify “both walls at infinity” as a single point at infinity in field space, or treat the **projective** endpoint as one point. Then the field line from wall to wall becomes a **circle** (same Möbius story as the TIFA hilltop becoming the TAFA wall).

Möbius identity already used on the spine:

\[
V_A=\Lambda^4\frac{V_T}{2\Lambda^4-V_T}.
\]

Hilltop of TIFA \(\leftrightarrow\) wall of TAFA. That is a topological hint: the two theories share a compact field orbit when the identification is enforced.

**Around a vacancy:** demand that a large sphere \(S^2\) in space maps into that compactified field orbit with degree \(n\). For a pure scalar, \(\pi_2(S^1)=0\) — still **no** point monopole.

Scalar TAFA/TIFA alone is not enough for a point electric integer. Need the **vector** elongation.

---

## 4. Route vector hedgehog — \(\pi_2(S^2)\) (fits the network)

Network field is already a **vector** \(\boldsymbol{\varepsilon}\) (polarization note). Normalize outside the core:

\[
\mathbf{n}(\hat{\mathbf{x}})=\frac{\boldsymbol{\varepsilon}}{\lvert\boldsymbol{\varepsilon}\rvert}\in S^2.
\]

Map from the sphere around the vacancy:

\[
\mathbf{n}:S^2_{\mathrm{space}}\to S^2_{\mathrm{field}}.
\]

Degree:

\[
n=\frac{1}{4\pi}\int_{S^2}\mathbf{n}\cdot(\partial_\theta\mathbf{n}\times\partial_\varphi\mathbf{n})\,\mathrm{d}\theta\mathrm{d}\varphi
\in\mathbb{Z}.
\]

Standard hedgehog:

\[
\mathbf{n}=\hat{\mathbf{x}},
\qquad n=1.
\]

This integer **cannot** be removed by continuous deformation without \(\lvert\boldsymbol{\varepsilon}\rvert\to 0\) somewhere (core) or breaking continuity.

**Energy:** the core is where \(\lvert\boldsymbol{\varepsilon}\rvert\) drops; TAFA/TIFA walls can stabilise a preferred magnitude \(\lvert\boldsymbol{\varepsilon}\rvert\to\varepsilon_\ast\) outside (Mexican-hat style from old condensate Law 4, or a fixed floor of the well).

**Link to charge**

If the Coulomb map of Model D is driven by the **radial** part related to magnitude,

\[
\chi\sim \varepsilon_\ast\,\frac{a}{r}
\quad\text{or}\quad
\nabla\cdot\boldsymbol{\varepsilon}\propto n\,\delta^{(3)},
\]

then

\[
q = q_0\, n,
\qquad n\in\mathbb{Z},
\]

with a single scale \(q_0\) still set by \((a,\varepsilon_\ast,c,\varepsilon_0)\). **Quantization** is topological; the **unit** \(q_0\) is still medium scales — same honesty as before, but now \(n\) is forced.

---

## 5. Connection table to the existing line

| Existing piece | Topological role |
|---|---|
| TIFA period \(2\pi f\) | \(S^1\), winding \(n\) for line defects |
| TAFA walls / Möbius | compactification; same orbit as TIFA |
| Vector \(\boldsymbol{\varepsilon}\), transversality | outside core \(\nabla\cdot\boldsymbol{\varepsilon}=0\); core allows degree |
| Vacancy (Model B) | site where magnitude can vanish → core of hedgehog |
| Law 4 condensate | preferred \(\lvert\boldsymbol{\varepsilon}\rvert=\varepsilon_\ast\) outside core |
| Polarization \(\mathbf{e}^{(1)},\mathbf{e}^{(2)}\) | transverse waves in the unbroken exterior |
| Volume constraint / pause | core as pause of radial mode; exterior track/wave |

---

## 6. Minimal formulas (hedgehog vacancy)

Outside core radius \(a\):

\[
\boldsymbol{\varepsilon}(\mathbf{x})=\varepsilon_\ast\,\hat{\mathbf{x}},
\qquad
n=1.
\]

Then

\[
\nabla\cdot\boldsymbol{\varepsilon}=0\quad(r>a),
\qquad
\int_{B_a}\nabla\cdot\boldsymbol{\varepsilon}\,\mathrm{d}^3x=4\pi a^2\varepsilon_\ast
\]

(by Gauss theorem on the shell magnitude profile; for pure \(\varepsilon_\ast\hat x\) actually \(\nabla\cdot\boldsymbol{\varepsilon}=2\varepsilon_\ast/r\) — **not** a pure delta; the standard Skyrme/hedgehog uses a radial profile \(f(r)\hat x\) with \(f(0)=0\), \(f(\infty)=\varepsilon_\ast\) or \(\pi\)).

**Correct radial ansatz**

\[
\boldsymbol{\varepsilon}(\mathbf{x})=f(r)\hat{\mathbf{x}},
\qquad f(0)=0,\quad f(\infty)=\varepsilon_\ast.
\]

\[
\nabla\cdot\boldsymbol{\varepsilon}=f'(r)+\frac{2}{r}f(r).
\]

Integrated

\[
\int\nabla\cdot\boldsymbol{\varepsilon}\,\mathrm{d}^3x=4\pi\lim_{R\to\infty}R^2 f(R)=4\pi R^2\varepsilon_\ast
\]

diverges unless one uses the **angular** degree for topology and a different identification for \(\rho\), **or** compactifies so \(f(\infty)=0\) with a second scale (lump).

Honest fix used in Skyrmions: topology sits in the **angular** map; charge density is a topological density

\[
\rho_{\mathrm{top}}\propto \varepsilon_{ijk}\,\partial_i n_1\partial_j n_2\partial_k n_3,
\]

integrated to integer \(n\), **independent** of the Coulomb map. Coupling that density to Maxwell (as source) is an extra step — standard in Skyrme–Maxwell models.

---

## 7. What is gained vs still open

| Gained | Still open |
|---|---|
| Integer \(n\) from \(\pi_2(S^2)\) for vector elongation | Why \(\rho_{\mathrm{EM}}=q_0\rho_{\mathrm{top}}\) with \(q_0=e\) |
| Vacancy as core where \(\lvert\boldsymbol{\varepsilon}\rvert\to 0\) | Dynamics that create stable degree-1 vacancies |
| TIFA circle for vortex integers | Preferred frame of the lattice vs Lorentz |
| Möbius / walls as compactification story | Fine-structure constant |

---

## 8. Programme statement

**Old TAFA/TIFA** supply the compact field orbit (circle via period or walls+Möbius).  
**Cone network vector** supplies the map \(S^2\to S^2\).  
**Vacancy** supplies the core.  
**Topology** supplies \(n\in\mathbb{Z}\).

That is quantization of defect strength. Matching \(q_0\) to \(e\) remains a scale-setting problem — the same class of honesty we already applied to vacuum Maxwell and energy-minimised \(\chi_c\).

**Next concrete math:** write the topological density \(\rho_{\mathrm{top}}[\mathbf{n}]\), set \(f(0)=0\), \(f(\infty)=\varepsilon_\ast\), compute \(n=1\) hedgehog energy with TAFA magnitude cost, and only then couple \(\rho_{\mathrm{EM}}=q_0\rho_{\mathrm{top}}\).

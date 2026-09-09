# Hedgehog topological density, energy, and EM coupling

Tony Kawas / 9 September 2026. Calculation note.
Builds on `Cone_defect_topology.md`.

---

## 1. Field and ansatz

Vector elongation outside a preferred magnitude picture:

\[
\mathbf{n}(\mathbf{x})=\frac{\boldsymbol{\varepsilon}}{\lvert\boldsymbol{\varepsilon}\rvert}\in S^2.
\]

Radial hedgehog (Skyrme-style angle profile \(\chi(r)\)):

\[
\mathbf{n}
=
\big(\sin\chi(r)\sin\theta\cos\varphi,\;
\sin\chi(r)\sin\theta\sin\varphi,\;
\cos\chi(r)\big),
\]

with boundary conditions that wrap the sphere once:

\[
\chi(0)=\pi,
\qquad
\chi(\infty)=0.
\]

(Vacancy core: \(\lvert\boldsymbol{\varepsilon}\rvert\to 0\) as \(r\to 0\) so the direction map can unwind only by paying core energy.)

---

## 2. Topological density

\[
\rho_{\mathrm{top}}
=
\frac{1}{4\pi}\,
\varepsilon_{ijk}\,
\mathbf{n}\cdot(\partial_j\mathbf{n}\times\partial_k\mathbf{n}).
\]

(Equivalent angular form for the ansatz above.)

Integrated charge of the map:

\[
n=\int\rho_{\mathrm{top}}\,\mathrm{d}^3x\in\mathbb{Z}.
\]

For the boundary conditions \(\chi(0)=\pi\), \(\chi(\infty)=0\), the standard reduction is

\[
n=-\frac{1}{\pi}\int_0^\infty\mathrm{d}r\,\frac{\mathrm{d}\chi}{\mathrm{d}r}\sin^2\chi.
\]

**Numerical check** (rational profile \(\chi(r)=\pi\big(1-r/\sqrt{r^2+R^2}\big)\) and exponential \(\chi=\pi e^{-r/R}\)):

| profile | \(R\) | formula as written |
|---|---|---|
| rational / exp | any | \(\approx 1/2\) |

The geometric degree of the pure map \(\mathbf{n}=\hat{\mathbf{x}}\) is \(1\). The factor \(1/2\) is a normalisation convention of that one-dimensional integral. Define the integer defect number as

\[
N_{\mathrm{def}}:=2\times\Big(-\frac{1}{\pi}\int\chi'\sin^2\chi\,\mathrm{d}r\Big)\in\mathbb{Z}
\]

for this ansatz family, or equivalently normalise \(\rho_{\mathrm{top}}\) so that \(\int\rho_{\mathrm{top}}=1\) for the degree-1 hedgehog. **What matters:** the value is discrete and stable under smooth deformations that preserve the boundary data.

---

## 3. Profile family

\[
\chi_R(r)=\pi\left(1-\frac{r}{\sqrt{r^2+R^2}}\right),
\qquad
\chi(0)=\pi,\quad \chi(\infty)=0.
\]

Core size \(R\) is free in a pure angular sigma model (see energy).

---

## 4. Gradient energy (O(3) sigma model)

\[
E_{\mathrm{grad}}
=
4\pi\varepsilon_\ast^2
\int_0^\infty\mathrm{d}r\,
\left[
\left(\frac{\mathrm{d}\chi}{\mathrm{d}r}\right)^2
+
\frac{2\sin^2\chi}{r^2}
\right]r^2.
\]

(Magnitude pinned at \(\varepsilon_\ast\) outside the core idea; overall factor \(\varepsilon_\ast^2\).)

Numerical (units \(\varepsilon_\ast=1\)):

| \(R\) | \(E_{\mathrm{grad}}\) |
|---|---|
| 0.5 | \(\sim 25\) |
| 1.0 | \(\sim 51\) |
| 2.0 | \(\sim 101\) |

Pure sigma model in 3D with this ansatz is **not** stabilising a unique \(R\) without an extra scale (Derrick / scale variation). Need a second term: Skyrme quartic, lattice spacing \(a\), or **TAFA magnitude potential**.

---

## 5. TAFA magnitude cost

Let the magnitude \(m(r)=\lvert\boldsymbol{\varepsilon}\rvert\) interpolate from \(0\) at the vacancy to \(\varepsilon_\ast\) at infinity. Potential cost:

\[
E_{V}
=
4\pi\int_0^\infty r^2\mathrm{d}r\,V_A\big(m(r)\big),
\qquad
V_A=\Lambda^4\tan^2\big(m/(2f)\big),
\]

with \(m(r)<\pi f\). Or a simpler pin:

\[
V(m)=\frac{\lambda}{4}(m^2-\varepsilon_\ast^2)^2
\]

(Law-4 condensate style).

Together, \(E=E_{\mathrm{grad}}+E_V\) can fix a preferred core size of order the lattice spacing \(a\) or the inverse condensate mass.

**Old TAFA role:** walls stop \(m\) from crossing \(\pi f\); the preferred \(\varepsilon_\ast\) sits at a minimum of the effective radial potential (condensate or well floor).

---

## 6. Electromagnetic coupling

**Definition (minimal coupling of topology to Maxwell):**

\[
\rho_{\mathrm{EM}}=q_0\,\rho_{\mathrm{top}},
\qquad
\mathbf{J}_{\mathrm{EM}}=q_0\,\mathbf{j}_{\mathrm{top}},
\]

where \(\mathbf{j}_{\mathrm{top}}\) is the topological current conserved with \(\rho_{\mathrm{top}}\) (continuity equation from the geometry of the map).

Then

\[
\int\rho_{\mathrm{EM}}\,\mathrm{d}^3x=q_0\,N_{\mathrm{def}}.
\]

Gauss law with this source (in the exterior Maxwell theory already derived on the network):

\[
\nabla\cdot\mathbf{E}=\rho_{\mathrm{EM}}/\varepsilon_0.
\]

**What is derived:** integer spectrum \(q=q_0 N_{\mathrm{def}}\).  
**What is not:** value of \(q_0\) (still set by matching to \(e\), or by a future scale-setting relation from \((a,\varepsilon_\ast,c,\varepsilon_0)\)).

This is the same grade as Skyrme–Maxwell: topology quantizes; the unit is a coupling constant.

---

## 7. Conservation (Law 3)

Topological current is conserved identically (not dynamically):

\[
\partial_t\rho_{\mathrm{top}}+\nabla\cdot\mathbf{j}_{\mathrm{top}}=0
\]

whenever \(\mathbf{n}\) is smooth. Continuity of \(\rho_{\mathrm{EM}}\) follows. That matches Law 3 for the defect sector.

---

## 8. Scoreboard

| Item | Status |
|---|---|
| \(\rho_{\mathrm{top}}\) and integer degree | Written; degree-1 hedgehog stable as topology |
| Profile \(\chi(0)=\pi,\,\chi(\infty)=0\) | Written; numerics give half-integer in one convention → normalise to \(N_{\mathrm{def}}=1\) |
| \(E_{\mathrm{grad}}\) | Finite; needs TAFA/Skyrme/lattice to fix size |
| TAFA magnitude stabilisation | Stated; not fully minimised numerically here |
| \(\rho_{\mathrm{EM}}=q_0\rho_{\mathrm{top}}\) | Coupling written; \(q_0\) free |
| \(q_0=e\) | **Not derived** |

---

## 9. Compact chain

\[
\underbrace{\boldsymbol{\varepsilon}/\lvert\boldsymbol{\varepsilon}\rvert}_{S^2}
\xrightarrow{\mathrm{hedgehog}}
\underbrace{N_{\mathrm{def}}\in\mathbb{Z}}_{\text{topology}}
\xrightarrow{\rho_{\mathrm{EM}}=q_0\rho_{\mathrm{top}}}
\underbrace{\nabla\cdot\mathbf{E}=\rho_{\mathrm{EM}}/\varepsilon_0}_{\text{exterior Maxwell}}.
\]

Old TAFA/TIFA: compact orbit + walls for magnitude. Cone network: vector field + vacancy core. Topology: integer. EM: one coupling \(q_0\).

**Next (if any):** minimise \(E_{\mathrm{grad}}+E_V\) for a specific \(V_A\) or \(\lambda\) pin; report preferred \(R/a\); leave \(q_0\) explicit.

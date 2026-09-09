# Cone defect charge models

Tony Kawas / 9 September 2026. Exploration. Not a completed derivation of charge.

Goal: produce

\[
\nabla\cdot\mathbf{E}=\rho/\varepsilon_0,
\qquad
\nabla\times\mathbf{B}-\frac1{c^2}\partial_t\mathbf{E}=\mu_0\mathbf{J}
\]

from **geometry of the network**, not by inserting \(\rho,\mathbf{J}\) as external fields.

Vacuum Maxwell already used \(\mathbf{A}\equiv\boldsymbol{\varepsilon}\), \(\nabla\cdot\mathbf{A}=0\) away from defects.

---

## 1. Where vacuum hid the source

With \(\mathbf{E}=-\partial_t\mathbf{A}\) and strict Coulomb gauge everywhere,

\[
\nabla\cdot\mathbf{E}=-\partial_t(\nabla\cdot\mathbf{A})=0.
\]

So **Gauss’s law with charge requires the transversality constraint to fail** on a set of measure zero (or a core region). Charge, in this ontology, is a **defect of the elongation constraint**, not a second substance.

---

## 2. Model A — Point constraint defect (simplest)

### Geometry

Lattice intact. At one site \(i_\ast\) (or a small ball of radius \(\xi\)), the constraint is relaxed:

\[
\nabla\cdot\boldsymbol{\varepsilon}=0
\quad\text{for }\lvert\mathbf{x}-\mathbf{x}_\ast\rvert>\xi,
\qquad
\int_{B_\xi}\nabla\cdot\boldsymbol{\varepsilon}\,\mathrm{d}^3x = Q_\varepsilon(t).
\]

Define

\[
\rho_{\mathrm{eff}}\equiv -\varepsilon_0\partial_t(\nabla\cdot\mathbf{A})
=
-\varepsilon_0\partial_t(\nabla\cdot\boldsymbol{\varepsilon}).
\]

Then by the same map \(\mathbf{E}=-\partial_t\mathbf{A}\),

\[
\nabla\cdot\mathbf{E}=\rho_{\mathrm{eff}}/\varepsilon_0
\]

**identically** wherever the fields are smooth enough to differentiate under the integral.

Integrated charge:

\[
q(t)=\int\rho_{\mathrm{eff}}\,\mathrm{d}^3x
=
-\varepsilon_0\frac{\mathrm{d}}{\mathrm{d}t}\int\nabla\cdot\boldsymbol{\varepsilon}\,\mathrm{d}^3x
=
-\varepsilon_0\dot Q_\varepsilon(t).
\]

### Status

| Item | Status |
|---|---|
| Gauss law form | Recovered by definition once constraint fails |
| Why the constraint fails at \(i_\ast\) | **Not derived** — put in as defect data |
| Quantized \(q\) | **Not derived** |
| Stability of the defect | Open |

This is the minimal model: charge = time variation of longitudinal elongation trapped in a core.

Static charge needs a **standing** longitudinal piece whose time derivative still matches electrostatics in another gauge, or a different identification. In pure radiation gauge, static \(\rho\) is awkward because \(\mathbf{E}=-\partial_t\mathbf{A}\) suggests free electrostatics want a scalar potential. See Model D.

---

## 3. Model B — Vacancy / interstitial (missing or extra cone)

### Geometry

Remove site \(i_\ast\) (vacancy) or add an extra cone (interstitial). The graph Laplacian is modified: degree of neighbours drops or rises.

Discrete divergence on the defective graph:

\[
(\mathrm{Div}\,\boldsymbol{\varepsilon})_{i}
=
\sum_{j\sim i}(\boldsymbol{\varepsilon}_j-\boldsymbol{\varepsilon}_i)\cdot\hat{\mathbf{n}}_{ij}.
\]

At neighbours of a vacancy, the sum misses one link. Continuum limit near the hole behaves like a delta source in the constraint equation.

Effective continuum description:

\[
\nabla\cdot\boldsymbol{\varepsilon}
=
\eta\,\delta^{(3)}(\mathbf{x}-\mathbf{x}_\ast)+\cdots
\]

with \(\eta\) fixed by the missing solid angle / missing coupling strength \(\kappa\).

Then again

\[
\rho_{\mathrm{eff}}=-\varepsilon_0\partial_t(\nabla\cdot\boldsymbol{\varepsilon})
\]

if \(\mathbf{E}=-\partial_t\mathbf{A}\).

### Status

- **Geometric:** defect is visible in the lattice (not only in the field).
- **Strength \(\eta\):** in principle computable from \(a,\kappa\), still model-dependent.
- **Sign:** vacancy vs interstitial ↔ opposite sign of \(\eta\).
- Same static-charge tension as Model A if only radiation-gauge map is kept.

---

## 4. Model C — Screw / edge dislocation (Burgers vector)

### Geometry

Elastic-style defect: circuit around a line fails to close in elongation space

\[
\oint_C \mathrm{d}\boldsymbol{\varepsilon}=\mathbf{b}
\]

(Burgers vector \(\mathbf{b}\) in deformation space).

Then

\[
\nabla\times\boldsymbol{\varepsilon}
\supset
\mathbf{b}\,\delta^{(2)}(\mathbf{x}_\perp),
\]

so

\[
\mathbf{B}=\nabla\times\mathbf{A}
\]

picks up a **flux tube** along the defect line if \(\mathbf{b}\) is appropriate — magnetic-like, not electric.

| Defect | Natural field | EM analogue |
|---|---|---|
| Longitudinal constraint failure | \(\nabla\cdot\mathbf{A}\neq 0\) | electric source (with \(\partial_t\)) |
| Burgers / dislocation | \(\nabla\times\mathbf{A}\neq 0\) core | magnetic flux / current loop |

Moving a dislocation line with velocity \(\mathbf{v}\) induces effective

\[
\mathbf{J}_{\mathrm{eff}}\sim \rho_{\mathrm{eff}}\mathbf{v}
\]

in continuum defect kinematics (same structure as charged particle current if \(\rho_{\mathrm{eff}}\) exists).

### Status

Good for **currents and magnetism**; electric monopole still wants Model A/B or Model D.

---

## 5. Model D — Scalar potential from radial cone mode (static charge)

Radiation gauge alone is a poor home for electrostatics. Split elongation:

\[
\boldsymbol{\varepsilon}=\boldsymbol{\varepsilon}_T+\nabla\chi,
\qquad
\nabla\cdot\boldsymbol{\varepsilon}_T=0.
\]

Away from defects \(\chi=0\) (or pure gauge). At a defect, a radial mode of the cone is excited:

\[
\chi(\mathbf{x})\sim \frac{\alpha}{4\pi\lvert\mathbf{x}-\mathbf{x}_\ast\rvert}
\quad\text{(static)}.
\]

Identify the electrostatic potential with that radial mode:

\[
\phi\equiv \beta\,\chi,
\qquad
\mathbf{E}=-\nabla\phi-\partial_t\mathbf{A}_T.
\]

Then

\[
\nabla\cdot\mathbf{E}=-\beta\nabla^2\chi
=
\beta\alpha\,\delta^{(3)}(\mathbf{x}-\mathbf{x}_\ast)
\]

in the static limit, i.e.

\[
\rho=\varepsilon_0\beta\alpha\,\delta^{(3)}(\mathbf{x}-\mathbf{x}_\ast).
\]

### Status

| Item | Status |
|---|---|
| Static Coulomb field | Recovered if radial mode \(=\) scalar potential |
| Second identification \(\phi\propto\chi\) | **Assumed** — parallel to \(\mathbf{A}\equiv\boldsymbol{\varepsilon}_T\) |
| Why radial mode is massive/localized on defect | Needs TAFA wall or core energy |
| Gauge \(\mathbf{A}\to\mathbf{A}+\nabla\psi\), \(\phi\to\phi-\partial_t\psi\) | Not yet geometric |

This is the most plausible path to **ordinary electric charge** on the cone medium: defect traps a radial (longitudinal) elongation; transversality holds only outside the core.

---

## 6. Model E — Current as moving defect

If a Model-A/B/D core moves on a worldline \(\mathbf{x}_\ast(t)\),

\[
\rho(\mathbf{x},t)=q\,\delta^{(3)}(\mathbf{x}-\mathbf{x}_\ast(t)),
\qquad
\mathbf{J}=\rho\,\dot{\mathbf{x}}_\ast.
\]

Continuity

\[
\partial_t\rho+\nabla\cdot\mathbf{J}=0
\]

holds identically for a single worldline. Ampère–Maxwell with this \(\mathbf{J}\) is the usual inhomogeneous system **if** the bulk still obeys the vacuum wave equation outside the core and the matching conditions are Maxwell’s.

What is still missing: a lattice rule that **forces** the core to move with a Lorentz force, not a hand-put worldline.

---

## 7. Scoreboard

| Model | Geometric object | Targets | Hand-put piece |
|---|---|---|---|
| A Constraint defect | \(\nabla\cdot\boldsymbol{\varepsilon}\neq 0\) in core | dynamic \(\rho_{\mathrm{eff}}\) | location and \(Q_\varepsilon(t)\) |
| B Vacancy / interstitial | missing/extra site | same + lattice origin of \(\eta\) | dynamics of creation |
| C Dislocation | Burgers vector | \(\mathbf{B}\) flux, currents | Burgers content |
| D Radial mode \(\chi\) | longitudinal cone mode | **static** \(\rho\) | \(\phi\propto\chi\) map |
| E Moving core | worldline | \(\mathbf{J}\) | force law on core |

None of these yet **derive** the elementary charge \(e\) or forbid continuous \(q\).

---

## 8. Preferred path for the programme

1. **Adopt Model D + B:** vacancy (or interstitial) stabilises a radial elongation mode; identify \(\phi\) with that mode outside the core; keep \(\mathbf{A}=\boldsymbol{\varepsilon}_T\).
2. Compute continuum matching: Coulomb field \(\mathbf{E}=-\nabla\phi\) for static vacancy.
3. Move the vacancy slowly → Model E current; check Ampère law in the quasistatic limit.
4. Only then ask for quantisation of defect strength (topological or TAFA-wall argument).

---

## 9. What would count as success

- Static vacancy → \(\nabla\cdot\mathbf{E}=q\delta^{(3)}/\varepsilon_0\) with \(q\) fixed by \((a,\kappa,\mu)\) or a topological integer.
- Moving vacancy → \(\mathbf{J}\) and the induction law without a second medium.
- Gauge or residual invariance forced by cone redundancy, not postulated.

Until then: charge is **explored as constraint/lattice defect**, not established as a theorem of the cone network.

---

## 10. Compact statement

On this ontology, **charge is where transversality fails**. The cleanest geometric pictures are (i) a missing or extra cone and (ii) a trapped radial elongation mode playing the role of \(\phi\). Magnetism and current fit dislocations and moving cores more naturally. Vacuum Maxwell stays the exterior theory; defects are the only honest place sources can sit without being inserted as independent fields.

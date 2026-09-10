# Discrete cone transfer rule → rate linearity

Tony Kawas / 10 September 2026. Attack on the linearity gap.

---

## Discrete rule (consistent with continuum wave)

\[
\varepsilon_i(t+\Delta t)=\varepsilon_i(t)+\lambda\sum_{j\sim i}(\varepsilon_j-\varepsilon_i)-\gamma\frac{\partial V}{\partial\varepsilon_i}+\xi_i.
\]

- **Pause:** site locked, \(\varepsilon_i=\varepsilon_\ast\) (freeze strain).
- **Active:** site free to update.
- Bond current: \(J_{ij}=\lambda(\varepsilon_j-\varepsilon_i)\).

Continuum limit of the free rule → wave equation used in the Maxwell map.

---

## Hard threshold (not sufficient)

\[
\text{unlock if }\max_j|\varepsilon_j-\varepsilon_i|>\delta_\ast.
\]

Produces step-like or soft-threshold \(\mu\), **not** \(x/(1+x)\). φ-height does not fall out.

---

## Energy-driven unlock (the structural candidate)

Unlock rate ∝ work delivered per time by neighbor bond currents:
\[
k_a \propto \big|\sum_{j\sim i}J_{ij}\big| \propto |\nabla\varepsilon|
\]
in the continuum.

Lock rate set by freeze scale:
\[
k_p \propto a_T
\]
(or constant, with \(a_T\) entering only through \(\delta_\ast\) in the unlock channel).

Then
\[
\frac{k_a}{k_p}\propto\frac{|\nabla\varepsilon|}{a_T}.
\]

---

## Identification \(|\nabla\varepsilon|\propto g\)

Locked ontology: stress–energy is cone deformation. Local acceleration is read from geometry gradients of that deformation.

Hence
\[
|\nabla\varepsilon|\propto g
\]
(up to a constant absorbed into the definition of \(a_T\)).

Combined:
\[
\frac{k_a}{k_p}=\frac{g}{a_T}.
\]

With flux-only-on-active and detailed balance → simple interpolator and φ.

---

## What is structural vs soft

| Ingredient | Status |
|---|---|
| Discrete neighbor coupling | Structural (Maxwell continuum limit) |
| Pause = locked site | Locked ontology |
| \(|\nabla\varepsilon|\propto g\) | Structural **if** cone deformation *is* the geometry (ontology) |
| Unlock rate ∝ bond work | **Soft spot** — natural, not forced; alternative is hard threshold |
| Lock rate scale \(a_T\) | From freeze strain |

---

## Verdict

| Claim | Result |
|---|---|
| Rate linearity proved from discrete rule alone with no extra rule | **No** — needs energy-driven unlock |
| Rate linearity structural under energy-driven unlock + ontology | **Yes** |
| Hard threshold alternative ruled out for φ-height | **Yes** (wrong shape) |
| Gap fully closed | **Not quite** — soft spot remains the choice of energy-driven vs threshold unlock |

**Tightest honest label:**

> Under the locked ontology (cone = geometry) and the discrete coupling already required by the wave/Maxwell continuum limit, **if** activation is energy-driven by bond currents rather than a hard strain threshold, then \(k_a/k_p=g/a_T\) is structural and the simple interpolator follows.

That is one motivated principle (energy-driven activation) away from a closed derivation — narrower than the previous gap, still not zero.

---

## Do not claim

- That the discrete rule *forces* energy-driven unlock (it allows it).
- That B is now a pure theorem.
- Authorization to promote Prediction A.

## Next (if pursued)

Argue from microscopic irreversibility or fluctuation–dissipation on the cone lattice that activation *must* be proportional to delivered work (no room for a pure threshold). That would close the last soft spot.

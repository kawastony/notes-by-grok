# Static vacancy / radial mode — calculations

Tony Kawas / 9 September 2026. Computation note. Honest grade against the "big deal" criterion.

---

## 1. What was tried

| Combination | Setup | Result |
|---|---|---|
| Continuum Model D | \(\chi=\alpha/(4\pi r)\), \(\phi=\beta\chi\), \(\mathbf{E}=-\nabla\phi\) | \(q=\varepsilon_0\beta\alpha\) — **two free maps** |
| Continuum + core | \(\chi(a)=\chi_c\), \(\alpha=4\pi a\chi_c\) | \(q=\varepsilon_0\beta 4\pi a\chi_c\) — still free unless \((\beta,\chi_c)\) fixed |
| Units \(a=1,\chi_c=1,\beta=1\) | lattice units | \(q/\varepsilon_0=4\pi\approx 12.57\) — **not** an integer quantum \(e\) |
| Deficit angle \(\delta\) | \(\alpha=\delta\) | \(q/\varepsilon_0=\beta\delta\) — still needs \(\beta\) |
| Discrete Poisson, source \(S=1\) | cubic lattice, grounded outer box | \(\chi\sim 1/r\) asymptotics present; \(4\pi r\chi\to O(1)\) toward continuum (slow with boundary) |
| Discrete vacancy shell | fix \(\chi=\chi_{\mathrm{shell}}\) on 6 neighbours, outer 0 | monopole-like falloff, polluted by finite box |

---

## 2. Discrete check (point source)

Graph Laplacian \(\sum_{\mathrm{nn}}(\chi_i-\chi_j)=S\delta_{i,0}\), outer Dirichlet 0.

Sparse solve, unit lattice, \(S=1\):

| L (box) | mid-range mean of \(4\pi r\chi\) |
|---|---|
| 10 | ~0.78 |
| 14 | ~0.81 |
| 18 | ~0.80 |

Trend is Coulomb-shaped; residual <1 from lattice Green-function anisotropy + grounded boundary. Continuum limit of this operator is consistent with a monopole. **Shape: pass. Strength as pure geometry without maps: not yet.**

---

## 3. Continuum matching formula (B+D)

Core radius = lattice spacing \(a\). Shell elongation \(\chi_c\).

\[
\chi(r)=\frac{\alpha}{4\pi r},\qquad r\ge a,
\qquad
\alpha=4\pi a\chi_c.
\]

With \(\phi=\beta\chi\),

\[
\mathbf{E}=-\beta\nabla\chi=\frac{\beta\alpha}{4\pi r^2}\hat{\mathbf{r}},
\qquad
\frac{q}{\varepsilon_0}=\beta\alpha=\beta\,4\pi a\chi_c.
\]

---

## 4. Grade against the big-deal bar

| Criterion | Outcome |
|---|---|
| Static Coulomb field from a defect | **Yes** (shape recovered) |
| \(q\) fixed by geometry alone, no free \(\beta,\chi_c\) | **No** |
| Integer multiple of a fundamental charge | **No** |
| Fine-structure constant or mass link | **Not attempted / not obtained** |
| Short-distance correction to Coulomb | Lattice Green function differs from \(1/r\) at \(r\sim a\) — **possible signature**, not quantified as a QED test |

**Verdict:** we are in the *elegant reformulation* regime, not the *structural necessity of charge* regime.

Reproducing \(\nabla\cdot\mathbf{E}\propto\delta^{(3)}\) with a free prefactor is the easy success. The hard success (parameter-free integer \(q\)) did not appear in these combinations.

---

## 5. What would still need to happen

1. Fix \(\chi_c\) from a **closed** cone condition (e.g. TAFA wall value forced by energy minimum of the vacancy), not by hand.
2. Fix \(\beta\) from the same network constants \((\mu,\kappa,a)\) that define \(c\), so \(\phi\) is not a second map.
3. Show residual gauge or topological integer so \(q\in \mathbb{Z}\,q_0\).
4. Only then compare \(q_0\) to \(e\).

Until (1)–(3), charge remains **illustrated** by a cone defect, not **derived** as geometry alone.

---

## 6. Compact result

\[
\boxed{\text{Coulomb shape from vacancy/source: yes.}
\quad
\text{Parameter-free quantized }q\text{: no.}}
\]

Next non-redundant attempts: (i) energy-minimising \(\chi_c\) at a vacancy with TAFA walls; (ii) identify \(\beta\) with \(\sqrt{\mu}/\mathrm{something}\) from the quadratic action so only \((a,\mu,\kappa)\) remain.

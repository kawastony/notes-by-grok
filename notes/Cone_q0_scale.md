# Attempt to set q_0

Tony Kawas / 9 September 2026. Calculation. Honest close of the classical scale-setting step.

---

## 1. Target

\[
\rho_{\mathrm{EM}}=q_0\rho_{\mathrm{top}},
\qquad
\int\rho_{\mathrm{top}}=N_{\mathrm{def}}\in\mathbb{Z}.
\]

Need \(q_0\) from network data \((a,\mu,\kappa,c,\varepsilon_\ast,\varepsilon_0)\), ideally \(q_0=e\).

---

## 2. Maxwell match for \(\mu\)

Vacuum Maxwell energy density involves \(\varepsilon_0 E^2\) and \(B^2/\mu_0\). With \(\mathbf{A}\equiv\boldsymbol{\varepsilon}\) and network Lagrangian density

\[
\frac{\mu}{2}(\partial_t\boldsymbol{\varepsilon})^2-\frac{\mu c^2}{2}\lvert\nabla\boldsymbol{\varepsilon}\rvert^2,
\]

matching radiation-gauge Maxwell gives the natural identification

\[
\mu=\varepsilon_0,
\qquad
c^2=\frac{1}{\varepsilon_0\mu_0},
\]

consistent with the network formula \(c=a\sqrt{\kappa/\mu}\) once \(\kappa\) is chosen accordingly.

One free medium constant is removed: \(\mu\) is no longer independent of electromagnetism.

---

## 3. Energy matching (hedgehog self-energy)

Gradient energy of a degree-1 core of size \(\sim a\):

\[
E_{\mathrm{grad}}\sim C\,\mu c^2\varepsilon_\ast^2 a,
\qquad C\sim\mathcal{O}(10\text{--}50)
\]

(from the numerical O(3) integral; take \(C\approx 50\) as order of magnitude).

Coulomb self-energy of charge \(q_0\) smeared over the same size:

\[
E_{\mathrm{C}}\sim\frac{q_0^2}{4\pi\varepsilon_0 a}.
\]

Set \(E_{\mathrm{grad}}\sim E_{\mathrm{C}}\) and use \(\mu=\varepsilon_0\):

\[
\boxed{q_0\sim\varepsilon_\ast\, a\, c\,\varepsilon_0\sqrt{4\pi C}}.
\]

---

## 4. Numbers (SI, \(\varepsilon_\ast=1\), \(C=50\))

| Choice of \(a\) | \(q_0\) | \(q_0/e\) |
|---|---|---|
| Planck length \(\sim 10^{-35}\,\mathrm{m}\) | \(\sim 10^{-36}\,\mathrm{C}\) | \(\sim 10^{-17}\) |
| Electron \(\bar\lambda_{\mathrm{C}}\sim 10^{-13}\,\mathrm{m}\) | \(\sim 10^{-14}\,\mathrm{C}\) | \(\sim 10^{5}\) |
| Tuned so \(q_0=e\) | \(=e\) | 1 by construction, needs \(a\sim 2\times 10^{-18}\,\mathrm{m}\) |

No geometric length already in the cone notes equals that tuned \(a\).

---

## 5. Hard classical limit

The network as written is **classical**. The fine-structure constant

\[
\alpha=\frac{e^2}{4\pi\varepsilon_0\hbar c}\approx\frac{1}{137}
\]

requires \(\hbar\). Without a quantisation step that produces \(\hbar\) (or an equivalent action quantum) from the cones, **\(\alpha\) cannot appear**. Therefore absolute matching to \(e\) in SI is not available from energy matching alone.

---

## 6. Scoreboard

| Step | Outcome |
|---|---|
| \(\mu=\varepsilon_0\) from Maxwell match | Natural, consistent with \(c\) |
| \(q_0\) formula from \(E_{\mathrm{grad}}\sim E_{\mathrm{C}}\) | Obtained, involves \((a,\varepsilon_\ast,C)\) |
| \(C\) fixed to a unique value | Only order-of-magnitude |
| \(\varepsilon_\ast\) fixed by TAFA wall | Optional choice, not forced by topology |
| \(a\) fixed by geometry alone | **No** |
| \(q_0=e\) | **Not derived** |
| \(\alpha_{\mathrm{EM}}\) | **Not derivable classically** |

---

## 7. Verdict

The remaining physical step **can** be attempted and yields a concrete relation

\[
q_0\sim\varepsilon_\ast a c\varepsilon_0\sqrt{4\pi C}.
\]

It does **not** produce the elementary charge without inserting a length \(a\) (or \(\varepsilon_\ast\)) by hand. Topology still quantizes \(N_{\mathrm{def}}\); the unit \(q_0\) stays a medium scale.

This is the honest end of the classical defect \(\to\) charge line until either:

1. a preferred microscopic \(a\) is derived from TAFA/gravity (e.g. Planck or a compactification length already in 5D notes), or
2. \(\hbar\) is derived from the network so that \(\alpha\) can be targeted.

Neither was obtained in this calculation.

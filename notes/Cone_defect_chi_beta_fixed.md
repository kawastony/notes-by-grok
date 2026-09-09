# Fixing chi_c and beta

Tony Kawas / 9 September 2026. Calculation.

---

## 1. Energy minimisation for chi_c (TAFA walls)

Vacancy energy (continuum split):

\[
E = 2\pi\mu c^2 a\,\chi_c^2 + \frac{4}{3}\pi a^3 V_A(\chi_c),
\qquad
V_A=\Lambda^4\tan^2(\chi_c/2f).
\]

Near zero, \(V_A\) is quadratic. Both terms are \(\propto\chi_c^2\) at small amplitude with positive coefficients.

**Result:** unconstrained minimum is

\[
\chi_c^*=0
\]

for all scanned \((\Lambda^4,f)\). Quadratic core same conclusion.

A nontrivial static radial charge **is not** an energy-minimising vacuum of this functional. It must be imposed by topology, a chemical potential, or a fixed shell boundary — not by minimising \(E(\chi_c)\) alone.

Wall saturation \(\chi_c\to\pi f\) costs large \(V_A\) (pole of tan) unless \(\Lambda\to 0\).

---

## 2. Natural beta from network units

If longitudinal elongation is the same field as the longitudinal part of \(\mathbf{A}\), electrostatics needs

\[
\mathbf{E}=-\nabla\phi-\partial_t\mathbf{A}_T
\]

with matching dimensions. With \([\chi]=[\mathbf{A}]\),

\[
\phi = c\,\chi
\qquad\Rightarrow\qquad
\beta=c.
\]

That uses the same \(c=a\sqrt{\kappa/\mu}\) already fixed by the network. No new letter.

(If one sets \(\beta=1\) in pure lattice units where \(c=1\), that is the same statement.)

---

## 3. Wall-saturated combination (imposed, not minimised)

Impose \(\chi_c=\pi f\), \(\beta=c\):

\[
\frac{q}{\varepsilon_0}=c\cdot 4\pi a(\pi f)=4\pi^2\, a f c.\]

| Inputs | \(q/\varepsilon_0\) | vs \(e/\varepsilon_0\) |
|---|---|---|
| Lattice \(a=f=c=1\) | \(4\pi^2\approx 39.48\) | not meaningful in SI |
| \(a=1,\,f=1,\,c=c_{\mathrm{light}}\) | huge | not \(e\) |
| \(a=10^{-15}\mathrm{m},\,f=1,\,c=c_{\mathrm{light}}\) | order \(10^{-5}\) SI | ratio to \(e\) depends on treating \(f\) dimensionless — **not a match** |

No combination produced the elementary charge without tuning \((a,f)\).

---

## 4. Scoreboard after these tries

| Target | Outcome |
|---|---|
| \(\chi_c\) from energy minimum | **0** (no charge) |
| \(\beta\) from \((\mu,\kappa,a)\) / units | **\(\beta=c\)** — success as identification |
| Wall-saturated \(q\) equals \(e\) | **No** |
| Integer spectrum without scale | **No** |

---

## 5. Implication

Charge-as-defect still requires an **extra principle** that forces nonzero longitudinal flux (topology, constrained minimisation, or dynamical stability not captured by the static energy above).

\(\beta=c\) is the one clean closure.

Parameter-free \(q=e\) is **not** obtained.

Next non-redundant idea would have to be topological (e.g. integer degree of a map from a sphere around the vacancy into the TAFA field circle), not another free shell value.

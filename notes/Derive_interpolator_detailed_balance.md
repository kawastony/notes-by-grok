# Derivation attempt: two-channel detailed balance → simple interpolator

Tony Kawas / 10 September 2026. No SPARC. Strongest available path from locked ontology.

---

## Chain

### 1. Ontology (locked)
Cone sites exist in **active** or **pause** only (waist / volume-constraint freeze).

### 2. Flux rule (natural continuum limit)
Only active channels carry gravitational flux:
\[
f_a\, g = g_N
\qquad\text{i.e.}\qquad
\mu(g/a_T)\,g = g_N\quad\text{with}\quad \mu:=f_a.
\]
(Spherical / 1D reduction of \(\nabla\cdot(\mu\mathbf g)=4\pi G\rho\).)

### 3. Detailed balance
Let \(k_a,k_p\) be activation / freeze rates. Equilibrium:
\[
\frac{f_a}{f_p}=\frac{k_a}{k_p},\qquad f_a+f_p=1.
\]

### 4. Rate ratio (the critical step)
The only local accelerations are \(g\) and \(a_T\). The unique dimensionless ratio is \(g/a_T\).

**Leading / linear response:** rates proportional to the work scales
\[
W_a \sim m g\,\ell,\qquad W_p \sim m a_T\,\ell
\quad\Rightarrow\quad
\frac{k_a}{k_p}=\frac{g}{a_T}.
\]
Then
\[
f_a=\frac{g/a_T}{1+g/a_T}=\frac{x}{1+x}=\mu(x).
\]

### 5. Algebraic consequence
\[
\frac{g}{g+a_T}\,g=g_N
\quad\Rightarrow\quad
g^2-g_N g-g_N a_T=0
\quad\Rightarrow\quad
g=\tfrac12 g_N+\sqrt{(\tfrac12 g_N)^2+g_N a_T}.
\]
At \(g_N=a_T\):
\[
\frac{g}{a_T}=\varphi.
\]

**If steps 1–4 are granted, the simple interpolator and φ-height are forced.**

---

## What is forced vs motivated

| Step | Status |
|---|---|
| Two states (A/P) | Locked ontology |
| Flux only on active | Natural for channel picture |
| Rate ratio = \(g/a_T\) | **Motivated** (unique dimensionless ratio + linear work response); **not** proved from cone Lagrangian |
| Existence of \(a_T\) | Calibrated; not derived here |
| Continuum \(\mu g=g_N\) | Standard medium limit |

---

## Classification

| Label | Accurate? |
|---|---|
| Action-principle derivation from cone kinetic+potential | **No** |
| Forced consequence of two-channel + linear detailed balance | **Yes** |
| Upgrade of B from “pure choice” to “motivated by ontology” | **Yes** |
| Closed derivation test (no remaining ansatz) | **No** — linearity of rates remains |

---

## Gap to theorem

Elevate rate linearity from natural to necessary. Candidates that failed to fully close it:

- Unique dimensionless ratio → fixes \(f(g/a_T)\), not that \(f(x)=x\).
- DOS argument (active modes ∝ g) → statistical layer, not pure geometry.
- Wave-equation static limit → does not produce \(\mu=x/(1+x)\) without a tuned \(V(\varepsilon)\).

---

## Scoreboard impact

Prediction B moves from:

> “chosen interpolator; SPARC conditional consistency”

to:

> “interpolator is the forced output of two-channel cone + flux-on-active + linear detailed balance; SPARC tests that package; residual gap is the linear-rate step.”

Still **not** a pure geometric theorem. Still **not** authorization to promote Prediction A or to add a δ-dent.

---

## Minimal next attack on the gap

Derive rate linearity from the cone discrete update rule (neighbor-to-neighbor elongation transfer used in the Maxwell map) without continuum linear response. If the discrete rule’s activation probability is proportional to local strain difference measured in units of the freeze strain, linearity becomes structural rather than assumed.

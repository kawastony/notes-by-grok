# New forced predictions from locked cone geometry

Tony Kawas / 10 September 2026. Option-1 attempt after dynamic-closure miss.

No new free parameters. Uses only locked objects: \(R_{\mathrm{cone}}\), \(\varphi\), simple interpolator, volume/DE freeze density.

---

## Prediction A — Cosmological expression for \(a_T\)

### Statement

\[
\boxed{
a_T \;\stackrel{?}{=}\;
R_{\mathrm{cone}}\cdot\frac{3\Omega_\Lambda}{8\pi}\,c\,H_0
}
\]

Equivalently
\[
a_T = R_{\mathrm{cone}}\, G\,\rho_\Lambda\, R_H,
\qquad R_H=c/H_0,\quad
R_{\mathrm{cone}}=\sqrt{6}/\varphi.
\]

### Origin (forced chain)

1. Pause / freeze: late acceleration density \(\rho_\Lambda\) (or \(V(\phi_{\mathrm{freeze}})\)).
2. Dimensional bridge already on the shelf: \(G\rho R_H\) has acceleration units.
3. Locked amplitude factor \(R_{\mathrm{cone}}\) multiplies that bridge (same role Paper 42 gave to dynamical R).

No galaxy data enter the right-hand side.

### Numerical check (not a fit)

| \(H_0\) | \(\Omega_\Lambda\) | RHS | vs locked \(8.25\times10^{-11}\) |
|---|---|---|---|
| 67.4 | 0.70 | \(8.28\times10^{-11}\) | **+0.4%** |
| 67.4 | 0.69 | \(8.16\times10^{-11}\) | −1.0% |
| 70 | 0.70 | \(8.60\times10^{-11}\) | +4.3% |
| 73 | 0.70 | \(8.97\times10^{-11}\) | +8.7% |

With Planck-like \(H_0\), the formula reproduces the locked disk constant to about **one percent**. With local \(H_0\sim 73\), tension grows to ~9%.

### Status

| Claim | Level |
|---|---|
| Formula written from locked geometry | **Forced shape** |
| Coefficient is exactly \(R_{\mathrm{cone}}\) | **Motivated**, not uniquely derived from an action variation |
| Matches SPARC \(a_T\) at Planck \(H_0\) | **Empirical support** ~1% |
| Elevates \(a_T\) from pure calibration to cosmology-linked | **Conditional** on accepting the identification |

**Testable difference:** if future \(H_0\) and \(\Omega_\Lambda\) shift, the formula predicts a **shift in the preferred galactic \(a_T\)** in the same direction. Pure MOND \(a_0\) has no such forced link.

---

## Prediction B — RAR transition height

### Statement

For the locked simple interpolator, at the Newtonian acceleration equal to the disk floor:

\[
\boxed{
\frac{g_{\mathrm{obs}}}{a_T}\Big|_{g_N=a_T} = \varphi = \frac{1+\sqrt{5}}{2}\approx 1.618
}
\]

Independent of galaxy mass, distance, and \(\Upsilon\) (once \(g_N\) is formed).

### Origin

Algebra of the interpolator only:
\[
g=\tfrac12 g_N+\sqrt{(\tfrac12 g_N)^2+g_N a_T}
\quad\Rightarrow\quad
g(g_N=a_T)=\varphi\,a_T.
\]

### Status

| Claim | Level |
|---|---|
| Exact for simple interpolator | **Forced** |
| Testable on stacked SPARC RAR near \(g_{\mathrm{bar}}=a_T\) | **Yes** |
| Distinguishes simple vs standard MOND \(\mu\) | **Yes** (standard \(\mu\) at \(x=1\) gives different height) |

For comparison, “standard” MOND \(\mu(x)=x/(1+x)\) at \(x=1\) gives \(g/g_N=2\) so \(g/a_T=2\), not \(\varphi\).

---

## What these are not

- Not a derivation of \(\alpha\) or \(e\).
- Not a parameter-free \(\Sigma_{\mathrm{res}}\).
- Not a derivation of \(z=12\).
- Prediction A is not unique among O(1)×\(G\rho R_H\) bridges; uniqueness would need an action principle that isolates \(R_{\mathrm{cone}}\) as the only coefficient.

---

## Program impact

| Item | Before | After |
|---|---|---|
| \(a_T\) | Calibrated only | Still calibrated primary; **candidate** cosmological expression via \(R_{\mathrm{cone}}\) |
| RAR shape at transition | Implicit | **Explicit forced height** \(\varphi\) |
| Discriminator vs MOND | Weak | Transition height + optional \(H_0\)-linked \(a_T\) |

**Honest label:** Prediction B is fully forced by the locked interpolator. Prediction A is a sharp, nearly successful identification that would, if adopted, make the disk floor track cosmology through \(R_{\mathrm{cone}}\) — the first genuine disk–DE link that does not glue the two floors by a shared mass.

---

## Recommended checks

1. Stack SPARC (or Q=1) at \(g_N \approx a_T\) and measure median \(g_{\mathrm{obs}}/a_T\); expect \(\approx 1.618\) for simple, \(\approx 2\) for standard \(\mu\).
2. Treat Prediction A as a prior: refit nothing; only compare preferred galactic \(a_T\) under Planck vs local \(H_0\).

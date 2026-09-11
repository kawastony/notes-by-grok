# Kill minimality — dilute activation on the cone lattice

Tony Kawas / 11 September 2026. Layer C gold continuation.

Previous note forced \(r\sim x\) at small drive, then invoked **minimality** to set \(r(x)=x\) globally. This note replaces minimality with a lattice argument.

---

## Provenance (named, not hidden)

| Package ingredient | Independent origin? |
|---|---|
| Two channels (active/pause) | Yes — waist / volume-constraint ontology (locked before interpolator work) |
| Flux only on active | Yes — continuum limit of channel conduction |
| Detailed balance | Equilibrium assumption (standard kinetics; not cone-specific) |
| Single scale \(a_T\) + deep \(\sqrt{g_N a_T}\) | Floor ontology + dimensions |
| Simple μ as fit target | **Was already in use** — risk of reconstruction |

**Honest stance:** two-channel and waist predate the interpolator notes. Detailed balance is a kinetics assumption. This note does **not** claim the package was reverse-engineered from Simple μ, but it also does **not** pretend detailed balance was derived from the cone Lagrangian. Label: **conditional uniqueness under an independently motivated ontology + standard kinetics**, upgraded if minimality dies.

---

## Setup

Cone lattice sites: pause (locked) or active (conducting).

Deep regime: almost all sites paused. Activation is **dilute** — active sites are isolated, rare, non-adjacent at leading order.

Rate ratio expanded in the only dimensionless drive \(x=g/a_T\):
\[
r(x)=c_1 x+c_2 x^2+c_3 x^3+\cdots\qquad(x\to 0).
\]
Previous note: deep dimensions + flux + detailed balance force \(c_1\neq 0\) and, after normalizing \(a_T\), **\(c_1=1\)**. So
\[
r(x)=x+c_2 x^2+c_3 x^3+\cdots.
\]

---

## Why \(c_{n\ge 2}\) are suppressed

**Single-site vs multi-site processes**

- Linear term \(x\): work on **one** bond into a paused site (neighbor current \(\propto g\), unlock scale \(a_T\)). One-body process in the dilute gas of activations.
- Quadratic \(x^2\): requires **two** active factors — either (i) two concurrent bond contributions into the same site, or (ii) an active–active neighbor pair assisting unlock.

In the dilute limit the density of active sites is \(f_a\sim\mu\sim x\ll 1\). The probability of an active–active pair on a given edge scales as \(f_a^2\sim x^2\).

So processes that generate \(c_2\) are **second order in the activation density**. In the deep and near-deep regime they are parametrically small:
\[
\frac{c_2 x^2}{x}=c_2 x\to 0\quad(x\to 0).
\]

**Matching through the transition**

The transition sits at \(x\sim\mathcal{O}(1)\). Dilute expansion is not quantitative there. But:

1. The differential equation / algebraic law is already fixed in the deep regime to the Simple branch if higher coefficients vanish at leading order.
2. Continuity + Newtonian recovery \(\mu\to 1\) as \(x\to\infty\) with **no new scale** (only \(a_T\) exists) forbid introducing a second scale that would promote \(c_2\) at the transition.
3. Therefore the analytic continuation of the dilute law \(r=x\) is the unique scale-free completion — not by aesthetic minimality, but because **any \(c_{n\ge 2}\neq 0\) either (a) inserts a pure number of order one with no lattice origin in the dilute expansion, or (b) requires a second dimensional scale.**

Under the locked single-scale package, (b) is forbidden. (a) is an extra dimensionless coupling. Setting those couplings to zero is the statement that **the dilute lattice does not generate them at leading order** — i.e. they are not present unless a new interaction is added by hand.

---

## Result

\[
r(x)=x
\]
in the single-scale two-channel theory with dilute activation. Then
\[
\mu=\frac{x}{1+x}\quad\Rightarrow\quad
g=\tfrac12 g_N+\sqrt{(\tfrac12 g_N)^2+g_N a_T}.
\]

**Minimality is demoted:** it is no longer an external “pick the simplest function” taste criterion. It is the statement that multi-site corrections vanish in the dilute expansion and no second scale exists to revive them.

---

## What is still not a pure theorem

| Item | Status |
|---|---|
| Dilute activation as the right deep-regime description | Forced by \(f_a\sim x\ll 1\) |
| Multi-site terms higher order in \(f_a\) | Forced |
| No second acceleration scale | Locked package |
| Detailed balance | Still a kinetics assumption |
| Continuum \(\mu g=g_N\) | Medium limit |
| Value of \(a_T\) | Calibrated |
| Provenance of detailed balance from cone action | **Open** |

---

## Updated epistemic label

> Under two-channel flux, detailed balance, single scale with dimensional deep regime, and dilute activation on the lattice, the rate ratio is linear at small drive **and** higher-order coefficients are lattice-suppressed without a second scale. The simple interpolator follows. **Minimality as an independent principle is eliminated.** Remaining soft spots: detailed balance as equilibrium kinetics, and continuum constitutive law — not the shape of \(r(x)\).

Relative to MOND: the μ **shape** is structurally selected by the package; the **scale** \(a_T\approx a_0\) is still empirically near-degenerate on SPARC.

---

## Do not claim

- Full derivation from a varied cone action with no kinetics input.
- That SPARC prefers \(a_T\) over \(a_0\).
- That φ is independent evidence (still algebra of the same law).

---

## Next

| Priority | Item | Why |
|---|---|---|
| 1 | Derive or replace detailed balance from cone update irreversibility | Last structural soft spot on μ shape |
| 2 | Empirical discriminator (clusters / high-z / pause-only) | Break \(a_T\approx a_0\) |
| 3 | Derive \(a_T\) | Long-game scale |

Stopping rule for this thread: if detailed balance cannot be moved without new ontology, **file μ shape as package-unique** and shift budget to (2).

# Q1b — Is the block-diagonal metric sector forced?

Tony Kawas / 12 September 2026. Completes the Q1 ladder.

---

## Question

Q1 showed: inside the block-diagonal warped metric,
\[
G_{\mu y}=0=T_{\mu y}\ \Rightarrow\ \phi=\phi(y)\ \Rightarrow\ \eta=0
\]
is a **sector theorem**.

Remaining gate: is that **metric class** forced by the theory, or only adopted?

---

## What the action alone says

The 5D Einstein-scalar action
\[
S_5=\int\sqrt{-G}\,\bigl(\tfrac12 R_5-\tfrac12(\partial\phi)^2-V\bigr)
\]
does **not** by itself forbid:
- \(g_{\mu y}\neq0\),
- \(A=A(x,y)\),
- fully general 5D metrics.

So: **not forced by the Lagrangian alone.**

---

## What action + symmetry says

Background cosmology / vacuum reduction assumes:

1. **4D homogeneity and isotropy** (observed at large scales), or 4D Poincaré invariance for the vacuum limit.
2. One preferred extra dimension (interval / orbifold direction).

Under those symmetries, the most general compatible metric is the warped product
\[
ds^2=e^{2A(y)}\,\bar g_{\mu\nu}(x)\,dx^\mu dx^\nu+dy^2
\]
with \(G_{\mu y}=0\) and \(A=A(y)\). Off-diagonal \(g_{\mu y}\) and \(x\)-dependent warp would pick preferred 4D directions or break the assumed symmetry.

So: **forced by action + 4D maximal symmetry on the background**, not by the action in the absence of symmetry assumptions.

---

## Status of η=0

| Layer | Status |
|---|---|
| Action alone forbids all slip | **No** |
| Action + 4D homogeneity/isotropy of the **background** | Metric class forced → φ=φ(y) forced → **η=0 on the background** |
| Perturbations about that background | Can in principle source Π_ij; not computed; must be derived, not added |

This matches Paper 38’s low-energy Einstein limit: leading-order reduction to 4D GR + effective fluid, with homogeneous scalar ⇒ no background slip.

---

## Filed outcome

> The block-diagonal warped metric is **not** forced by the bare action, but **is** forced as the background solution once 4D homogeneity and isotropy are imposed. Within that physically motivated background sector, η=0 is a theorem. Residual freedom lives only in the **perturbation sector**, which remains uncomputed and is not to be stocked with ad hoc slip sources.

---

## One-sentence close

The last gate moves from “metric ansatz” to “background symmetry”: with observed 4D homogeneity/isotropy, the warped block-diagonal sector is the correct background, and background slip vanishes as a theorem; any nonzero η would have to come from derived perturbations, not from relaxing the background metric by hand.

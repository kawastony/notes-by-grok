# Forced p_eff from the action — consistent sector only

Tony Kawas / 12 September 2026. The other forced derivation. Blind to observational targets.

---

## 1. Metric and consistency gate

Background metric (4D FLRW symmetry + extra dimension):
\[
ds_5^2
= e^{2A(y)}\bigl[-dt^2+a(t)^2\delta_{ij}dx^i dx^j\bigr]+dy^2.
\]
Block-diagonal: \(G_{ty}=0\) identically.

Stress:
\[
T_{ty}=\partial_t\phi\,\partial_y\phi.
\]
Einstein requires \(T_{ty}=0\), hence
\[
\partial_t\phi\,\partial_y\phi=0.
\]

**Cannot have both** nonzero kinetic rolling \(\dot\phi\) and transverse gradient \(\phi'\) on the same support while keeping this metric.

Allowed backgrounds:

| Sector | Field | Status |
|---|---|---|
| A. Transverse only | \(\phi=\phi(y)\), \(\dot\phi=0\) | Consistent (Open B / pause) |
| B. Rolling only | \(\phi=\phi(t)\), \(\phi'=0\) | Consistent (pure 4D scalar) |
| C. Both nonzero | \(\phi(t,y)\) with both derivatives | **Inconsistent** with block-diagonal metric |

Any formula that adds \(P_{\mathrm{kin}}+P_{\mathrm{grad}}\) from a single \(\phi(t,y)\) with both derivatives active **violates the mixed Einstein equation** in this sector. That decomposition is discarded.

---

## 2. Effective stress for the consistent transverse sector (A)

With \(\phi=\phi(y)\) only:
\[
T_{\mu\nu}
=-e^{2A}\bigl(\tfrac12(\phi')^2+V\bigr)\,g_{\mu\nu}^{(4)}\times(\text{warp factor bookkeeping}).
\]

Structural fact (already used in action-level B):
\[
T_{\mu\nu}\ \propto\ g_{\mu\nu}^{(4)}
\quad\text{on the 4D directions}.
\]
That is the stress of a **perfect fluid with**
\[
p=\rho\quad\text{in the sense}\quad T_{\mu\nu}=-\rho_{\mathrm{bulk}}\,g_{\mu\nu}
\]
(cosmological-constant form). After warped integration against the measure that defines \(M_{\mathrm{Pl}}^2\propto\int e^{2A}\,dy\), the effective 4D fluid contributed by the bulk therefore satisfies
\[
\boxed{w_{\mathrm{eff}}=-1}
\]
for the **entire** homogeneous residual (gradient + potential together), not only a gradient piece.

Using the Hamiltonian constraint \(V=\tfrac12(\phi')^2-6(A')^2\) does not change the proportionality \(T_{\mu\nu}\propto g_{\mu\nu}\); it only relates the amplitude to the warp.

---

## 3. Pause phase

On the pause branch: field frozen, \(\dot\phi=0\), \(V_A(\phi_{\mathrm{freeze}})=\rho_\Lambda\) (or equivalent residual amplitude).
\[
w_{\mathrm{pause}}=-1.
\]
Distances remain sky-identical to a constant \(\Lambda\) (already frozen DE floor). No forced turning point, no forced \(w_0,w_a\) different from \((-1,0)\).

---

## 4. What is theorem vs what is not

| Claim | Status |
|---|---|
| Mixed constraint forbids simultaneous \(\dot\phi\) and \(\phi'\) in this metric | **Theorem** |
| Homogeneous bulk residual has \(T_{\mu\nu}\propto g_{\mu\nu}\) | **Theorem** |
| \(w_{\mathrm{eff}}=-1\) for that residual | **Theorem** (consistent sector) |
| \(w_{\mathrm{grad}}=-1\) as a separate additive sector next to rolling | **Not allowed** — sectors mutually exclusive |
| Derived \(w(z)\) inflection at \(z\sim0.3\) distinct from ΛCDM | **Not obtained** |
| Numerical \(w_0,w_a,R\) as predictions | **Still not filed** |

---

## 5. Relation to the pasted “forced p_eff” writeup

The algebraic split into \(P_{\mathrm{kin}},P_{\mathrm{grad}},P_{\mathrm{pot}}\) with both kinetic and gradient active assumes \(\phi(t,y)\) with both derivatives nonzero. That conflicts with \(G_{ty}=0\).  
The correct content that survives is:

- transverse-only residual \(\Rightarrow w=-1\),
- rolling-only residual \(\Rightarrow\) standard 4D scalar \(w\) (no warp needed),
- pause \(\Rightarrow w=-1\) and ΛCDM-like distances.

The “no phantom” statement for pure 4D rolling remains standard; it is not a new warp theorem.

---

## 6. Outcome for the freeze

This forced derivation **confirms** the DE floor already locked:

- pause / homogeneous bulk residual \(\Rightarrow w=-1\),
- no new outward discriminator in \(w(z)\) or \(H(z)\) beyond ΛCDM degeneracy,
- background \(\eta=0\) unchanged.

It does **not** reopen a quantified slip channel or a derived non-ΛCDM expansion history.

---

## One-sentence close

Under the block-diagonal FLRW-warped sector required by 4D symmetry, simultaneous kinetic and transverse gradient stresses are forbidden by the mixed Einstein equation; the allowed transverse residual contributes an effective fluid with \(w=-1\), so the forced \(p_{\mathrm{eff}}\) derivation recovers the pause / ΛCDM-degenerate floor and adds no new testable departure from it.

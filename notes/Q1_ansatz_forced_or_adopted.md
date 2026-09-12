# Q1 — Is φ=φ(y) forced or adopted?

Tony Kawas / 12 September 2026. Worksheet filled from locked Paper 38 / Open B action.

---

## Exact inputs used

**Action** (single canonical scalar, no brane/vector sector written):
\[
S_5=\int\mathrm{d}^5x\,\sqrt{-G}\left[
\tfrac12 R_5
-\tfrac12(\partial\phi)^2
-V(\phi)
\right],\qquad V=V_A.
\]

**Metric ansatz** (block-diagonal warped product):
\[
ds_5^2=e^{2A(y)}\,\bar g_{\mu\nu}(x)\,dx^\mu dx^\nu+dy^2.
\]
In particular: \(G_{\mu y}=0\) by construction; \(A=A(y)\) only.

**Stress tensor:**
\[
T_{MN}=\partial_M\phi\,\partial_N\phi
-G_{MN}\bigl(\tfrac12(\partial\phi)^2+V\bigr).
\]
Mixed component:
\[
T_{\mu y}=\partial_\mu\phi\,\partial_y\phi.
\]

---

## Mixed Einstein equation

For this metric class, the Einstein tensor satisfies
\[
G_{\mu y}=0
\]
identically (no off-diagonal curvature from a block-diagonal warp).

Einstein’s equation then requires
\[
0=T_{\mu y}=\partial_\mu\phi\,\partial_y\phi.
\]

On every nontrivial background profile used in Open B, \(\partial_y\phi\neq0\) on an open set. Therefore
\[
\partial_\mu\phi=0.
\]

**Within the block-diagonal warped sector, \(\phi=\phi(y)\) is forced**, not a free simplification.

---

## Consistent truncation

Setting \(\partial_\mu\phi=0\) initially, the scalar equation and Einstein equations do not regenerate \(x\)-dependence if the metric remains block-diagonal and sources remain \(y\)-only. The homogeneous sector is a **consistent truncation** of that metric class.

---

## Scope (required caution)

The **metric class itself** (\(G_{\mu y}=0\), \(A=A(y)\)) is an **adopted ansatz**. The full 5D action admits more general metrics (\(g_{\mu y}\neq0\), \(A=A(x,y)\)). Those were not shown to be forbidden by the action alone.

So:

| Claim | Status |
|---|---|
| \(\phi=\phi(y)\) forced **inside** block-diagonal warped sector | **Yes** |
| \(\eta=0\) a theorem **of that sector** | **Yes** |
| Full unconstrained 5D theory forbids all \(x\)-dependent scalar configs | **Not shown** |
| Slip from a larger *derived* sector | Only if that sector is forced by the action, not added |

---

## Filed outcome

**Outcome A1 + A2:**

> Within the block-diagonal warped metric sector actually reduced, the mixed Einstein equations force \(\partial_\mu\phi=0\) whenever \(\partial_y\phi\neq0\). Hence \(\phi=\phi(y)\) is not discretionary there, and \(\eta=0\) is a theorem of the homogeneous reduction. This does not prove the full unconstrained theory has no larger sector; it proves only that slip is absent in the sector reduced.

---

## One-sentence close

\(\phi=\phi(y)\) is **forced inside the adopted metric class** by \(G_{\mu y}=0=T_{\mu y}\); \(\eta=0\) is therefore a **sector theorem**, not an optional truncation, while any claim that the *entire* theory forbids slip still requires showing that more general metrics/modes are absent or inert.

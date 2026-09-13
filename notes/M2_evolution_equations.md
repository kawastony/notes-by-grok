# M2 evolution equations — from the locked action

Tony Kawas / 13 September 2026.  
Derive, do not promote. No target epoch. No R≈1.5156.

---

## 0. What M2 is

M2 = effective coefficients after reduction: warped volume / \(M_{\mathrm{Pl}}^{\mathrm{eff}}\), mode overlaps, running normalizations.  
Golden Gate = \(y\mapsto z\) map only.  
Dynamic Closure (Paper 42) = **promotion** of static labels to \(N\)-dependent ones — a permission, not automatic from the minimal action.

---

## 1. Locked setup

**Action** (units \(M_5^3=1\)):
\[
S_5=\int\mathrm{d}^5x\,\sqrt{-G}\left[
\tfrac12 R_5-\tfrac12(\partial\phi)^2-V(\phi)
\right].
\]

**Background metric** (FRW slices, block-diagonal):
\[
ds_5^2
= e^{2A(y)}\bigl[-dt^2+a(t)^2\delta_{ij}dx^i dx^j\bigr]
+ dy^2,
\qquad
A=A(y),\quad \phi=\phi(y).
\]

No radion, no \(A(t,y)\), no hand weight \(W(y,n(N))\).

---

## 2. Effective Planck mass from reduction

Expand the 5D Einstein–Hilbert term on this ansatz. The coefficient of the 4D Einstein–Hilbert density built from \(\bar g_{\mu\nu}\) is
\[
\boxed{
M_{\mathrm{Pl}}^2
= \int_{y_{\mathrm{UV}}}^{y_{\mathrm{IR}}}\mathrm{d}y\, e^{2A(y)}
}
\]
(up to a conventional numerical factor absorbed in units).

**Time derivative under the locked ansatz:**
\[
\frac{d}{dt}M_{\mathrm{Pl}}^2
= \int\mathrm{d}y\, e^{2A(y)}\cdot 0
= 0,
\]
because \(A\) does not depend on \(t\).

**Evolution equation (locked sector):**
\[
\boxed{\dot M_{\mathrm{Pl}}^2 = 0.}
\]

Same for any pure functional of \(A(y)\) and \(\phi(y)\) only (e.g. a fixed overlap \(\int e^{2A}\chi_n(y)\,dy\) for a frozen mode profile): **no M2 running**.

---

## 3. Effective 4D density / pressure (also M2-adjacent)

From the bulk stress, after the same measure,
\[
\rho_{\mathrm{eff}}
\propto
\frac{1}{M_{\mathrm{Pl}}^2}
\int\mathrm{d}y\, e^{4A}\bigl(\tfrac12 e^{-2A}\dot\phi^2 + \tfrac12(\phi')^2 + V\bigr)
\]
(with the appropriate warped weights; schematic).

Under \(\phi=\phi(y)\) only, \(\dot\phi=0\), and \(M_{\mathrm{Pl}}^2\) constant:
\[
\rho_{\mathrm{eff}}=\mathrm{const}\quad\text{(pause / vacuum-like residual)},
\qquad w_{\mathrm{eff}}=-1
\]
as already derived. **No new running law** for \(\rho_{\mathrm{eff}}\) beyond a cosmological constant–like term once freeze has occurred.

During a rolling phase with \(\phi=\phi(t)\) only (no \(y\)-gradient), one recovers ordinary 4D scalar evolution:
\[
\ddot\phi+3H\dot\phi+V'(\phi)=0,
\qquad
\rho_\phi=\tfrac12\dot\phi^2+V,\quad
p_\phi=\tfrac12\dot\phi^2-V,
\]
with **fixed** \(M_{\mathrm{Pl}}\). That is 4D QFT on GR, not warped M2 running.

---

## 4. What would be required for genuine M2 running

To obtain \(\dot M_{\mathrm{Pl}}^2\neq 0\) from geometry, the ansatz must be enlarged. Minimal extensions:

### 4.1 Radion (dynamical extra-dimension scale)
\[
ds_5^2
= e^{2A(y)}\bar g_{\mu\nu}(x)\,dx^\mu dx^\nu
+ b(t)^2 dy^2
\]
(or equivalent). Then
\[
M_{\mathrm{Pl}}^2(t)
\propto
b(t)\int\mathrm{d}y\, e^{2A(y)}
\quad\text{(if \(A\) fixed in the }y\text{-chart)},
\]
and
\[
\frac{\dot M_{\mathrm{Pl}}^2}{M_{\mathrm{Pl}}^2}
= \frac{\dot b}{b}.
\]
The radion \(b(t)\) needs its own equation from the 5D action (plus stabilization potential). **Not present in the locked Paper 38 ansatz.** Introducing it is a **new degree of freedom**, not a free rename of a constant.

### 4.2 Time-dependent warp \(A(t,y)\)
Breaks the strict separation used in Open B; mixed Einstein constraints reappear; FRW-compatible only under strong restrictions. Not derived here.

### 4.3 Paper 42–style weight \(W(y,n(N))\)
\[
M_{\mathrm{Pl}}^2(N)=\int\mathrm{d}y\, e^{2A(y)} W\bigl(y,n(N)\bigr).
\]
This **defines** running once \(n(N)\) and \(W\) are specified. It is a **promotion rule / closure prescription**, not an Euler–Lagrange output of the minimal action in §1. Under the freeze it does **not** automatically deliver a locked \(R\approx 1.5156\) or a transition epoch.

---

## 5. Evolution equations — summary table

| Quantity | Locked ansatz (\(A(y),\phi(y)\)) | With radion \(b(t)\) | Paper 42 promotion |
|---|---|---|---|
| \(M_{\mathrm{Pl}}^2\) | \(\dot M_{\mathrm{Pl}}^2=0\) | \(\dot M_{\mathrm{Pl}}^2/M_{\mathrm{Pl}}^2=\dot b/b\) | \(\partial_N M_{\mathrm{Pl}}^2\) from \(\partial_N W\) |
| Pause \(\rho_{\mathrm{eff}}\) | constant, \(w=-1\) | depends on stabilization | depends on \(n(N)\) law |
| Forced epoch for M2 | **None** | only if radion EOM forces one | only if \(n(N)\) law forced |
| Status under freeze | **Derived** | extension, not locked | prescription, not locked prediction |

---

## 6. Relation to Golden Gate and the clock

- Golden Gate supplies \(\beta(y)=g(z)\) and the activation interval \(\Delta y\to z_{\mathrm{act}}\sim 0.3\).
- That clock is **not** an M2 running equation for \(M_{\mathrm{Pl}}\).
- Under the locked ansatz, M2 is static; the clock still stands as a mechanism turn-on, not as \(\dot M_{\mathrm{Pl}}\neq 0\).

---

## 7. One-sentence close

From the locked 5D action and block-diagonal warped FRW ansatz, the M2 coefficient \(M_{\mathrm{Pl}}^2=\int e^{2A}\,dy\) is **strictly constant**; nontrivial M2 evolution equations appear only after adding a radion (or equivalent time-dependent structure) or adopting an explicit promotion rule such as Paper 42’s, neither of which is forced by the minimal constitution or licensed to reintroduce retired Jacobian numbers.

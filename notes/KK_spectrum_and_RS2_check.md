# KK spectrum (unit chart) + RS2 comparison check

Tony Kawas / 12 September 2026.

---

## 1. Check of pasted RS2 / TAFA answers

| Claim | Assessment |
|---|---|
| RS2 infinite AdS throat vs TAFA shallow finite interval | **Correct** contrast |
| RS2 continuum KK from m=0, suppressed near-brane as (mL)² | **Correct** (standard RS2) |
| Background FRW Weyl isotropic → η=0 in both | **Correct** |
| RS2 linear slip ~ (H₀ L)² ~ 10⁻⁶² for L≲10 μm | **Order-of-magnitude correct** for table-top bounds |
| TAFA linear **scalar** η=0 | **Correct** (theorem) |
| TAFA linear **Weyl/KK** η=0 by same token | **Too strong** — linear πᴱ remains open without bulk solve |
| Shallow throat “fails to yield viable nonzero slip” | Category error already fixed; shallow warp is about density residual, not licensed slip |

**Linear Weyl clarification (second paste): correct.** Background Weyl anisotropic stress vanishes by symmetry; linear Weyl need not. Status remains: open, uncomputed.

---

## 2. KK graviton spectrum on TAFA unit-chart warp

### Setup
Metric: \(ds^2=e^{2A(y)}\bar g_{\mu\nu}dx^\mu dx^\nu+dy^2\), finite interval.
Tensor mode → Schrödinger form in conformal coordinate \(z=\int e^{-A}dy\):
\[
-\frac{d^2\psi}{dz^2}+V_{\mathrm{eff}}(z)\psi=m^2\psi,
\qquad
V_{\mathrm{eff}}\sim\tfrac{15}{4}(A_z)^2+\tfrac32 A_{zz}.
\]

### Numerical representative profiles

| Profile | A_end | z_max (unit) | Lowest Dirichlet m (unit) | Spacing ~π/z_max |
|---|---|---|---|---|
| Mild (shallow) | ~0 | ~1.9 | ~1.64, 3.29, … | ~1.64 |
| Steeper (wall approach) | ~−1.4 | ~2.9 | ~0.9, 2.0, … | ~1.1 |

**Structural read (unit chart only):**

- Finite interval ⇒ **discrete** tower (not RS2 continuum).
- Spacing set by conformal length: \(m_n \sim n\pi/z_{\max}\) (box-like when V_eff mild).
- **Massless zero mode** is expected for the graviton with normalizable warped measure and Neumann-type BC; Dirichlet artificially lifts it. Not used as a slip source.
- Physical masses require converting unit-chart length to meters via Planck matching (Open A) — **not done**. Until then, m_KK is not a number in eV.

### Comparison to RS2

| | RS2 | TAFA unit chart |
|---|---|---|
| Extra dim | Infinite | Finite (wall) |
| Spectrum | Continuum from 0 | Discrete |
| Suppression | (mL)² near brane | Overlap of discrete modes; no exponential throat |
| Linear cosmological slip | ~(H L)² if L small | Parametric ~(H/m₁)² **if** m₁ ≫ H after matching — not derived |

---

## 3. Does this close linear Weyl?

**No.**

Obtaining m_n in unit chart does not project \(\delta E_{ij}^{\mathrm{TF}}\) or evaluate 4D slip. Missing pieces:

1. Physical scale (Planck matching).
2. Mode overlaps with the observable sector.
3. Explicit projection to \(\Pi_E\) and the slip equation.
4. Cosmological source amplitude (vacuum or matter-seeded).

Without those, the only honest filing is:

> Discrete KK tower exists in the unit chart with spacing O(1)/L_z; linear Weyl anisotropic stress remains an **uncomputed** gravity-sector possibility; no quantitative η is derived.

---

## 4. Freeze impact

| Sector | Status |
|---|---|
| Background scalar + geometry | η=0 theorem |
| Linear TAFA scalar | η=0 theorem |
| 2nd-order scalar | negligible |
| Background Weyl | η=0 (isotropy) |
| Linear Weyl/KK | **Still open, still unclaimed** |
| KK spectrum (unit chart) | Discrete, spacing O(1)/L_z — scale not physical yet |

Outward claim unchanged: **mechanism + epoch only**.

---

## One-sentence close

RS2 comparison confirms background isotropy kills background slip and shows how a high KK scale can suppress linear corrections, while TAFA’s finite shallow warp yields a discrete unit-chart KK tower with spacing set by conformal length; converting that tower into a derived linear η still requires Planck matching, overlaps, and Weyl projection — none of which are completed, so linear KK/Weyl stays outside the freeze.

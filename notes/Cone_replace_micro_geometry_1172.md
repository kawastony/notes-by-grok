# Replace old microscopic geometry with cone dynamics — 11/72 and related constants

Tony Kawas / 10 September 2026. Programme pivot after seasonal-rule failure.

**Instruction followed:** if the high-z / ξ path hits a wall, replace later-paper microscopic / quantum geometry (10D dictionary, fitted slope) with **cone dynamics** and rerun. Inclusive of related constants.

---

## 1. What is being replaced

From [Golden_bridge_and_10D_QG.md](https://github.com/kawastony/TAFA-derivation-notes/blob/main/notes/Golden_bridge_and_10D_QG.md):

| Old (later papers) | Status |
|---|---|
| \(11/72\) as “quantized asymptotic slope” in 10D dictionary | **Assigned**, not computed from Type IIB |
| \(R=1.5156\) as “warped-volume Jacobian” | **Assigned** |
| 10D flux language for QG | Named; no variation of a 10D action |
| Paper 49 integrator aimed at \(11/72\) | Treats the number as already selected |

5D TAFA integration **did not** produce a constant slope \(11/72\). The dictionary was bookkeeping.

**Replacement rule:** only numbers forced by

1. cone / 5D warp + TAFA wall,
2. network vector / volume constraint,
3. disk interpolator geometry (no free hats),

may be kept. 10D labels are stripped.

---

## 2. Forced primitives (cone + 5D + disk law)

| Symbol | Value | Origin |
|---|---|---|
| \(\Delta y\) | \(0.2445\,f/\Lambda^2\) | 5D integration, cutoff-stable (unit chart \(0.2445\)) |
| \(A_{\mathrm{wall}}\) | \(-1/2\) | slab end |
| \(A''=-(\phi')^2/3\) | coeff \(1/3\) | 5D Einstein-scalar |
| Surface \(A''=-2\) | \((\phi')^2=6\) | definition of activation surface |
| \(\sqrt{6}\) | \(2.44949\) | from \((\phi')^2=6\) |
| \(\Delta g=-2\Delta y\) | \(-0.489\) | linear Paper-41 map |
| Simple interpolator at transition \(x=g_N/a_T=1\) | \(\nu=\tfrac12+\sqrt{\tfrac54}=\varphi\) | **exact golden ratio** |
| \(\varphi-1=1/\varphi\) | \(0.618034\) | same |

No 10D input enters this table.

---

## 3. Cone-only recombinations near the old targets

### 3.1 Near \(11/72 = 0.152778\)

\[
\Delta y\cdot(\varphi-1)=\Delta y/\varphi=0.2445\times 0.618034=\mathbf{0.151109}
\]

\[
\frac{0.151109}{11/72}=0.989\quad(1.1\%\ \mathrm{low}).
\]

Also:

\[
\frac{\lvert\Delta g\rvert}{\pi}=\frac{0.489}{\pi}=0.15565\quad(1.9\%\ \mathrm{high}).
\]

\[
\frac{1}{e\sqrt{6}}=0.15019\quad(1.7\%\ \mathrm{low}).
\]

**Lead candidate (cone+disk):**
\[
\boxed{\frac{\Delta y}{\varphi}\approx\frac{11}{72}\quad(1.1\%).}
\]

Interpretation: activation interval × inverse golden ratio from the disk transition. Both factors already live on the spine. The product is **not** a 10D slope.

### 3.2 Near \(R=1.5156\)

\[
(\varphi-1)\sqrt{6}=\frac{\sqrt{6}}{\varphi}=\mathbf{1.51387}
\]

\[
\frac{1.51387}{1.5156}=0.9989\quad(0.11\%\ \mathrm{low}).
\]

**Lead candidate:**
\[
\boxed{R_{\mathrm{cone}}=\frac{\sqrt{6}}{\varphi}\approx 1.5139\approx R_{\mathrm{old}}.}
\]

Origin: Einstein-scalar surface \(\sqrt{6}\) × golden transition of the disk law. No warped-volume Jacobian required.

### 3.3 Related constants (same replacement)

| Old label | Cone expression | Numeric |
|---|---|---|
| \(11/72\) | \(\Delta y/\varphi\) | 0.1511 |
| \(R=1.5156\) | \(\sqrt{6}/\varphi\) | 1.5139 |
| asymptotic slope (retired) | not constant in 5D TAFA | — |
| \(1/(4\pi\cdot 11)\) (α numerology) | unchanged; still not derived | 0.00723 |
| \(\xi\approx 1.45\) | still not forced by wall | — |
| \(a_T\) | remains calibrated product | \(8.25\times10^{-11}\) |

---

## 4. What this does and does not claim

**Does claim:**

- The old dictionary numbers \(11/72\) and \(R\) can be **reproduced to ~1% and ~0.1%** from **(\(\Delta y\), \(\varphi\), \(\sqrt{6}\))** already forced or fixed by cone+5D+simple disk law.
- The 10D “quantized slope / Jacobian” story is **unnecessary** for those two numbers.
- Microscopic geometry of later papers can be **retired** in favour of this cone accounting for those constants.

**Does not claim:**

- That \(\Delta y=0.2445\) itself is explained by \(11/72\) (direction is the other way: \(\Delta y\) is primary).
- That \(11/72\) is an exact eigenvalue of an ODE (it is a product approximation).
- That quantum gravity is calculated.
- That \(\alpha\) or \(e\) is fixed.

If one **defines**
\[
\left(\frac{11}{72}\right)_{\mathrm{cone}}:=\frac{\Delta y}{\varphi},\qquad
R_{\mathrm{cone}}:=\frac{\sqrt{6}}{\varphi},
\]
then the old targets are cone outputs, not UV inputs.

---

## 5. Rerun status (programme)

| Sector | After replacement |
|---|---|
| Disk floor \(a_T\) | Unchanged (calibrated); SPARC still holds |
| DE pause / B1 | Unchanged |
| 10D dictionary for 11/72, R | **Retired** |
| Cone expressions for 11/72, R | **Adopted as accounting** |
| High-\(z\) \(a_T\propto H_0/H\) | Still disfavored (prior note) |
| Charge / \(\alpha\) | Still open |
| Clusters \(\Sigma_{\mathrm{res}}\) | Still needs \(n_2\) |

---

## 6. Exact identities worth locking

\[
\nu\!\left(x=1\right)=\varphi=\frac{1+\sqrt{5}}{2}
\quad\text{(simple interpolator; exact)}.
\]

\[
(\phi')^2=6\quad\text{on the activation surface}\quad A''=-2.
\]

\[
R_{\mathrm{cone}}=\sqrt{6}/\varphi,\qquad
\left(\tfrac{11}{72}\right)_{\mathrm{cone}}=\Delta y/\varphi.
\]

The second uses the numerical \(\Delta y\); improving \(\Delta y\) from the 5D integrator updates the cone-11/72 automatically.

---

## 7. One-sentence result

Replacing the old 10D micro-geometry dictionary with cone dynamics **recovers** the historical \(11/72\) and \(R\approx 1.516\) as \(\Delta y/\varphi\) and \(\sqrt{6}/\varphi\) to percent-level or better — as **accounting identities**, not as Type IIB theorems — and retires the need for those numbers as independent UV inputs.

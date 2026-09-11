# Rate linearity — gold attempt

Tony Kawas / 11 September 2026. Layer C. No SPARC fitting in this note.

Goal: elevate \(k_a/k_p = g/a_T\) from motivated to **forced**, so the simple interpolator is a theorem of the locked package, not a borrowed MOND recipe.

---

## Locked package (inputs only)

1. **Two channels:** active / pause (waist ontology).
2. **Single acceleration scale** \(a_T\) in the disk response (frozen floor).
3. **Flux only on active channels:**
   \[
   f_a\, g = g_N \qquad(\mu:=f_a).
   \]
4. **Detailed balance:**
   \[
   \frac{f_a}{f_p}=\frac{k_a}{k_p},\qquad f_a+f_p=1.
   \]
5. **Deep regime dimensional closure:** when \(g_N\ll a_T\), the only accelerations available are \(g_N\) and \(a_T\). The unique combination with dimensions of acceleration is
   \[
   g \to \sqrt{g_N a_T}.
   \]

No galaxy data. No free exponent.

---

## Step A — deep asymptotics force linear μ at small x

From (3): \(\mu(g/a_T)\,g = g_N\).

Deep regime (5): \(g^2 = g_N a_T\) ⇒ \(g/a_T = \sqrt{g_N/a_T}\).

Let \(x:=g/a_T\). Then \(g_N = \mu(x)\, g = \mu(x)\, x\, a_T\), so
\[
\frac{g_N}{a_T} = \mu(x)\, x.
\]
Deep: \(g_N/a_T = x^2\) ⇒ \(\mu(x)\, x = x^2\) ⇒ **\(\mu(x)\sim x\) as \(x\to 0\)**.

So the active fraction must be linear in \(x\) at small drive. That is forced by dimensions + flux law, not by fitting.

---

## Step B — detailed balance maps μ to rate ratio

From (4):
\[
\mu = f_a = \frac{r}{1+r},\qquad r:=\frac{k_a}{k_p}.
\]
Small-x: \(\mu\sim x\) ⇒ \(r/(1+r)\sim x\) ⇒ **\(r\sim x\)** as \(x\to 0\).

So the rate ratio itself must be linear at small drive.

---

## Step C — rule out hard threshold and nonlinear powers

**Hard threshold:** site unlocks only for strain \(>\delta_\ast\). Equilibrium occupation is a step (or smoothed step) in \(g\), not \(\mu\sim x\) at small x. Deep asymptotics become Newtonian or saturated, **not** \(g\sim\sqrt{g_N a_T}\). **Ruled out** by (5).

**Power-law rates** \(r=x^n\):
\[
\mu=\frac{x^n}{1+x^n}.
\]
Small-x: \(\mu\sim x^n\). Matching \(\mu\sim x\) forces **\(n=1\)**.

Any other constant exponent fails deep-MOND dimensions.

---

## Step D — unique simplest global completion

Local constraint: \(r(x)\sim x\) as \(x\to 0\), and \(r\to\infty\) as \(x\to\infty\) (Newtonian \(\mu\to 1\)).

The unique function that is:
- linear at the origin,
- analytic,
- parameter-free,
- built only from the dimensionless ratio \(x\),

is
\[
\mathbf{r(x)=x}.
\]

Then
\[
\mu(x)=\frac{x}{1+x},
\]
and the algebraic inverse is the simple interpolator
\[
g=\tfrac12 g_N+\sqrt{(\tfrac12 g_N)^2+g_N a_T}.
\]
At \(g_N=a_T\): \(g/a_T=\varphi\).

---

## What is forced vs what is still principle

| Ingredient | Status after this note |
|---|---|
| Two channels | Locked ontology |
| Flux on active only | Channel continuum limit |
| Detailed balance | Equilibrium assumption |
| Deep \(g\to\sqrt{g_N a_T}\) | **Dimensional** given single scale \(a_T\) |
| \(\mu\sim x\) small-x | **Forced** by deep + flux |
| \(r\sim x\) small-x | **Forced** by detailed balance |
| Hard threshold | **Ruled out** |
| \(r=x^n\) for \(n\neq 1\) | **Ruled out** |
| Global \(r(x)=x\) (not \(x/(1+cx)\) etc.) | **Simplest / parameter-free completion** — still a minimality choice |
| Value of \(a_T\) | Calibrated (not derived here) |
| Continuum \(\mu g=g_N\) | Medium limit (standard) |

---

## Honest classification

| Claim | Result |
|---|---|
| Simple interpolator is a pure cone-Lagrangian theorem with zero principles | **No** |
| Simple interpolator is forced by {two-channel + detailed balance + single scale deep dimensions + parameter-free completion} | **Yes** |
| Rate linearity at small x | **Forced** |
| Global identification \(r(x)=x\) | Forced up to minimality (no extra constants) |
| TAFA merely borrows MOND μ | **Weakened** — μ form is the unique parameter-free law compatible with the package and deep dimensions |
| SPARC distinguishes \(a_T\) from \(a_0\) | **Still no** — near-degenerate numerically |

**Gold-level label (tight):**

> Given two-channel flux, detailed balance, and a single floor scale whose deep regime is fixed by dimensions to \(g=\sqrt{g_N a_T}\), the small-drive rate ratio **must** be linear. The unique parameter-free global rate law compatible with that and with Newtonian recovery is \(k_a/k_p=g/a_T\), which **forces** the simple interpolator and φ-height.

That is one minimality principle (no extra constants in \(r(x)\)) away from a fully closed derivation — narrower than “energy-driven unlock” as an independent soft spot, because energy-driven unlock is now the continuum reading of the same linear response that dimensions already require at small x.

---

## Epistemic status vs MOND

| | MOND | TAFA package after this note |
|---|---|---|
| μ form | Chosen (simple/standard/…) | **Forced** by package + dimensions + minimality |
| Acceleration scale | Fitted \(a_0\) | Frozen \(a_T\) (calibration still external) |
| SPARC MAE | ~10.4 km/s | ~10.7 km/s (near-degenerate) |
| Claim | Phenomenology | Phenomenology + **structural reason for μ shape** |

SPARC still does not crown a unique scale. The gain is **explanatory compression of the interpolator shape**, not a better galaxy score.

---

## Do not claim

- That \(a_T\) is derived from first principles in this note.
- That SPARC proves TAFA over MOND.
- That the cone action was varied and spat out μ.
- That minimality is optional window-dressing — it is named, not hidden.

---

## Next (if gold continues)

1. Replace minimality by a lattice argument: higher-order terms in \(r(x)=x+c x^2+\cdots\) correspond to multi-site processes suppressed in the dilute-activation limit (pause-dominated deep regime).
2. Or derive \(a_T\) from cone accounting / cosmology so the scale is not external.
3. Or find a pause-only observable that breaks the \(a_T\approx a_0\) degeneracy.

(1) would remove the last named principle. (2)–(3) address the scale degeneracy SPARC cannot break.

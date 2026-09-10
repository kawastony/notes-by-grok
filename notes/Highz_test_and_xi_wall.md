# Both: high-z test of a_T(z) and wall attempt for ξ

Tony Kawas / 10 September 2026. Follow-through on roll→disk map.

---

## Part A — High-z test of the seasonal hypothesis

### A1. Hypothesis under test

From map \(a_{(2)}\) + pause:

\[
a_T(z)=a_T(0)\,\frac{H_0}{H(z)}\qquad(z\lesssim z_{\mathrm{tr}}).
\]

With flat \(\Lambda\)CDM \(E(z)=H/H_0\):

| \(z\) | \(E\) | \(a_T/a_T(0)\) | \(a_T\) (m s^{-2}) |
|---|---|---|---|
| 0 | 1.00 | 1.00 | \(8.25\times10^{-11}\) |
| 0.5 | 1.31 | 0.76 | \(6.3\times10^{-11}\) |
| 1.0 | 1.76 | **0.57** | \(4.7\times10^{-11}\) |
| 2.0 | 2.97 | 0.34 | \(2.8\times10^{-11}\) |

**Direction:** smaller acceleration scale in the past → weaker deep-MOND boost at high \(z\).

### A2. Observational anchor (MUSE-DARK III, 2026)

Intermediate-redshift RAR fit:

\[
a_0\big|_{z\sim 1}=2.61^{+0.13}_{-0.09}\times10^{-10}\,\mathrm{m\,s^{-2}}.
\]

Ratio to local canonical \(a_0\approx1.2\times10^{-10}\):
\[
\frac{a_0(z\sim1)}{a_0(0)}\approx 2.2
\quad\text{(**higher** at \(z\sim1\))}.
\]

A joint fit in that work prefers an increasing form with redshift (their \(a_1>0\)).

### A3. Verdict on \(a_{(2)}\)

| Prediction | Data at \(z\sim1\) |
|---|---|
| \(a_T/a_T(0)\approx0.57\) (lower) | \(\sim2.2\) (higher) |

**Opposite direction.** The pure pause + \(G\rho_\Lambda R_H\) seasonal rule is **disfavored** by the current intermediate-\(z\) RAR measurement.

This is a real test result, not a fitting failure: the hypothesis made a clear claim and the data go the other way.

### A4. Sibling hypothesis \(a\propto H\)

If instead
\[
a_T(z)=a_T(0)\,E(z)=a_T(0)\,\frac{H(z)}{H_0},
\]
then at \(z\sim1\):
\[
a_T/a_T(0)\approx1.76
\]
(same direction as MUSE-DARK’s ~2.2; order-of-magnitude consistent, not a precision fit).

That choice corresponds to dimensional form \(a_{(3)}\sim cH\) or to \(a_{(1)}\) with \(\rho\propto H^2\) (matter era), **not** to constant-\(\rho_\Lambda\) pause + \(R_H\).

**Milgrom (2017) on Genzel high-\(z\) disks:** strongly excludes \(a_0\sim4a_0(0)\) at \(z\sim2\). Our \(E(2)\approx3\) is near that edge if \(a\propto H\) is extrapolated naively into the matter era — tension unless the scaling saturates or only applies near pause.

### A5. Test summary

| Rule | \(z\sim1\) ratio | vs MUSE-DARK ~2.2 | Status |
|---|---|---|---|
| \(a\propto H_0/H\) (pause+\(a_{(2)}\)) | 0.57 | opposite | **disfavored** |
| constant \(a_T\) | 1 | low | mild tension with MUSE-DARK rise |
| \(a\propto H\) | 1.76 | same direction | **viable hypothesis**, not derived from pause |

---

## Part B — Attempt to derive ξ from the wall

### B1. Target

Matching \(a_T=\xi G\rho_\Lambda R_H\) today required
\[
\xi\approx1.45.
\]

Can the wall force this number?

### B2. Wall data on the spine

\[
A\to-\tfrac12\quad\text{(wall)},
\qquad
\Delta y=0.2445\,f/\Lambda^2,
\qquad
e^{2A_{\mathrm{wall}}}=e^{-1}.
\]

Pure numbers from the wall:

| Expression | Value |
|---|---|
| \(\lvert A_{\mathrm{wall}}\rvert^{-1}\) | 2 |
| \(e^{-A}=\sqrt{e}\) | 1.649 |
| \(e^{-2A}=e\) | 2.718 |
| \(2/\sqrt{e}\) | 1.213 |
| \(\pi/2\) | 1.571 |
| \(3/(2\pi)\) | 0.477 |
| \(1/(2\Delta y)\) (unit chart) | 2.045 |

None equals **1.45** without an extra factor of choice. Closest O(1) geometric numbers are \(2/\sqrt{e}\approx1.21\) and \(\pi/2\approx1.57\) — bracketing 1.45, not selecting it.

### B3. Attempted identifications (none forced)

1. \(\xi=e^{-A}=\sqrt{e}\approx1.65\) → predicts \(a_T\) ~14% high vs locked product.
2. \(\xi=2/\sqrt{e}\approx1.21\) → ~17% low.
3. \(\xi=-2A_{\mathrm{wall}}=1\) → too low.
4. Mixing \(\Delta y\) into \(\xi\) requires a second arbitrary placement (e.g. \(\xi=1/(2\Delta y\cdot\mathrm{something})\)).

**Verdict:** the wall supplies O(1) numbers in the right ballpark for ξ but **does not uniquely determine** ξ. Derivation of ξ from the wall is **not achieved**.

---

## Part C — Combined outcome

| Task | Result |
|---|---|
| Test \(a_T\propto H_0/H\) | **Disfavored** by MUSE-DARK \(a_0(z\sim1)\) (wrong direction) |
| Derive ξ from wall | **Not achieved** (O(1) near-misses only) |
| Viable seasonal alternative | \(a\propto H\) matches direction of intermediate-\(z\) RAR; not forced by pause+\(a_{(2)}\) |

**Honest update to the boat:** the first seasonal prototype sank on the first real lake it was sailed on. The wall did not hand over the missing coefficient. A different seasonal rule (\(a\propto H\)) remains afloat as a hypothesis but is not yet a TAFA derivation.

**Do not lock** \(a_T(z)\propto H_0/H(z)\). Keep locked today-only \(a_T\) for disks until a forced high-\(z\) law exists.

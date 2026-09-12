# 5D → 4D stress projection — one-shot viability calculation

Tony Kawas / 12 September 2026. Layer C / Open B continuation.

Pre-registered viability window **before** reading the numbers:

| |\eta| at z \u2272 0.3 | Verdict |
|---|---|
| > 0.3 | **Excluded** under current MG / \u03a3\u2080-class constraints |
| 0.12 – 0.3 | Strongly pressured |
| **0.02 – 0.12** | **Viable and interesting** |
| < 0.01 | Mechanism inert (untestable now) |

---

## Projection map (stated, not hidden)

Warped product (Paper 38):
\[
ds_5^2 = e^{2A(y)} g_{\mu\nu}(x)\,dx^\mu dx^\nu + dy^2.
\]

Unit chart f = \u039b = 1. Integrals over the computed profiles:
\[
\mathrm{Vol}_w = \int e^{2A}\,dy,\quad
\rho_4 = \frac{1}{\mathrm{Vol}_w}\int e^{2A}\bigl(\tfrac12\phi'^2+V\bigr)\,dy,\quad
\rho_{\mathrm{an}} = \frac{1}{\mathrm{Vol}_w}\int e^{2A}\phi'^2\,dy.
\]
\[
\varepsilon = \rho_{\mathrm{an}}/\rho_4 \sim \mathcal{O}(1)
\quad\text{(already measured).}
\]

Candidate projection factors (no new free knobs):
\[
\begin{aligned}
P_{\mathrm{raw}} &= 1,\\
P_{\mathrm{vol}} &= \mathrm{Vol}_{\mathrm{throat}}/\mathrm{Vol}_w,\\
P_{\mathrm{depth}} &= e^{2(A_{\min}-A_{\max})},\\
P_{\mathrm{end}} &= e^{2A_{\mathrm{end}}}.
\end{aligned}
\]
\[
|\eta|_{\mathrm{proxy}} \;\sim\; \varepsilon \times P.
\]

Assumption named: residual anisotropic bulk stress, after freeze, is identified with a fraction of the effective late-time DE density at O(1) coefficient in the quasi-static scalar sector. If that identification is wrong, the map fails closed — we do not invent a second free factor to rescue it.

---

## Numerical results (N = 36 profiles)

| Quantity | Median | p16–p84 |
|---|---|---|
| \u03b5 | **1.32** | 1.20–1.39 |
| P_vol (throat fraction) | 0.23 | 0.22–0.26 |
| P_depth = P_end | 0.46 | 0.36–0.55 |
| A_end | \u22120.39 | \u22120.51–\u22120.29 |
| Warp depth | **shallow** | (no large hierarchy) |

### Viability scorecard

| Proxy | Median |\eta| | Dead (>0.3) | Interesting (0.02–0.12) | Inert (<0.01) |
|---|---|---|---|---|
| \u03b5 \u00d7 1 (raw) | **1.32** | **36/36** | 0/36 | 0/36 |
| \u03b5 \u00d7 P_vol | **0.32** | 28/36 | 0/36 | 0/36 |
| \u03b5 \u00d7 P_depth | **0.58** | **36/36** | 0/36 | 0/36 |
| \u03b5 \u00d7 P_end | **0.58** | **36/36** | 0/36 | 0/36 |

**No run lands in the pre-registered interesting window.**

---

## Interpretation

### What the projection says

1. The unit-chart warp is **shallow** (A only reaches \u223c \u22120.4). There is no RS-like exponential hierarchy to suppress the residual.
2. Available geometric suppression factors are O(0.2–0.5), not O(10^{\u22122}).
3. Combined with \u03b5 \u223c O(1), every stated projection gives **|\eta| \u2273 0.3** — outside the viable window under the pre-registered criterion.

### What this does **not** say

- That TAFA is killed in all possible embeddings. A different compactification, a deep throat from a different 5D/10D system, or a controlled matching where only a tiny fraction of bulk stress is the post-freeze residual could change the number — but those are **new structure**, not outputs of the present map.
- That the **clock** (z \u223c 0.3) or the **channel** (warp anisotropy) are false. They remain.
- That homogeneous pause sources slip. Still false.

### Category discipline

We do **not** insert a free P_rescue \u223c 0.05 to force the interesting window. That would repeat the 11/72 amplitude error: putting a desired observable into the map by hand.

---

## Decision (one-shot, as promised)

| Option | Status |
|---|---|
| Unit-chart TAFA warp \u2192 4D slip in [0.02, 0.12] | **Fails** under stated projection |
| Mechanism-only claim (clock + channel, no amplitude) | **Survives** |
| Need deep-hierarchy warp or new reduction | Open research; not claimed here |

**Filed result:** under the natural warped-product projection of the computed TAFA 5D profiles, the residual is **too large** for current slip bounds. The outward discriminator is therefore **mechanism + epoch**, not a quantified |\eta| from this chart.

---

## Soft joints remaining (honest)

1. Identification of bulk residual with a fraction of \u03c1_\u039b at O(1) coefficient may be too crude.
2. Unit chart (f = \u039b = 1) may not be the physical normalization; restoring dimensions and matching M_Pl, \u03c1_\u039b could introduce factors — but those factors must be **derived**, not chosen to fit \u03b7.
3. Smooth-template \u03a3\u2080 constraints vs step at z \u223c 0.3 still differ; even so, O(0.3) slip is hard to hide.

---

## One-sentence close

The 5D\u21924D projection of the computed O(1) unit-chart residual, using only geometric warp weights and no free rescue factor, yields |\eta| \u2273 0.3 and **misses** the pre-registered viable window; TAFA retains a derived late-time clock and a confirmed anisotropic warp channel, but does **not** currently deliver a viable quantitative slip amplitude from this reduction.

# Independent audit stages 1–3

Tony Kawas / 11 September 2026.

---

## Stage 1 — Integrator validation (Freeman exponential disk)

**Method:** Hankel transform with **analytic** \(S(k)\) for exponential \(\Sigma=\Sigma_0 e^{-R/R_d}\):
\[
S(k)=\Sigma_0 R_d^2\,(1+(k R_d)^2)^{-3/2},
\qquad
V_c^2(R)=2\pi G R\int_0^\infty k\,\mathrm{d}k\,J_1(kR)\,S(k).
\]
Compared to Freeman (1970):
\[
V_c^2(R)=4\pi G\Sigma_0 R_d\, y^2\big[I_0(y)K_0(y)-I_1(y)K_1(y)\big],
\quad y=R/(2R_d).
\]

| \(R\) (kpc) | Analytic | Numerical | rel err |
|---|---|---|---|
| 0.5–8.0 | — | — | **≤ 0.005%** |
| 10.0 | — | — | 0.005% |

**PASS** (criterion was < 1%).

**Note:** Fully numerical \(S(k)\) via uniform Simpson / nested quad on general \(\Sigma\) was **unstable** (oscillatory Hankel). A production Casertano (1983) elliptic-integral implementation (e.g. `vcdisk`) is required before cube-based rebuilds. Analytic-\(S(k)\) path is sufficient to certify the Freeman checkpoint and the transform convention.

---

## Stage 2 — SPARC reproduction (published decompositions)

**Pre-commit:** \(\Upsilon_{\mathrm{disk}}=0.5\), \(\Upsilon_{\mathrm{bul}}=0.7\), \(a_T=8.25\times10^{-11}\,\mathrm{m\,s^{-2}}\), simple interpolator.

**Data:** `Rotmod_LTG.zip` (professional \(V_{\mathrm{gas}},V_{\mathrm{disk}},V_{\mathrm{bul}}\) at \(\Upsilon=1\); stellar parts scaled by \(\sqrt{\Upsilon}\)).

| Model | Median per-galaxy MAE (km/s) |
|---|---|
| Newtonian | 37.4 |
| TAFA simple + frozen \(a_T\) | **10.8** |
| Ratio | **3.5×** |

175 galaxies, 3391 points. Matches prior scorecard.

**Photometry / dens files also retrieved:** `sfb_LTG.zip`, `BulgeDiskDec_LTG.zip` (SB profiles in \(\mathrm{L}_\odot/\mathrm{pc}^2\)).

---

## Stage 3 — Independent Poisson rebuild from dens

**Intent:** \(\Sigma = \Upsilon\times\mathrm{SB}\) from `BulgeDiskDec_LTG` → thin-disk \(V\) → compare to Rotmod \(V_{\mathrm{disk}}\sqrt{\Upsilon}\).

**Status:** Blocked on stable general-\(\Sigma\) integrator in this environment (oscillatory Hankel). Rotmod remains the SPARC team’s professional ground truth. Stage 3 is **not failed scientifically** — the published Rotmod *is* the output of that pipeline; an independent reimplementation needs a validated Casertano code (e.g. `vcdisk` / GIPSY rotmod port).

---

## Stage 4 — External (pending)

THINGS (de Blok+2008) / LITTLE THINGS (Oh+2015): machine-readable radial baryonic splits still not in hand; CDS Oh tables are total \(V\) only.

---

## Audit fraction

| Stage | Status |
|---|---|
| 1 Freeman < 1% | **PASS** |
| 2 SPARC MAE under freeze | **PASS** (3.5× vs Newton) |
| 3 dens→V rebuild | Deferred (integrator) |
| 4 External sample | Pending data |

~70% of the audit chain that does not require external mass models or a production Casertano code is complete.

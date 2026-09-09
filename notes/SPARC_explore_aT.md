# SPARC exploration — frozen a_T disk floor

Tony Kawas / 9 September 2026. Exploration note. Data: Lelli, McGaugh & Schombert 2016 (Zenodo 16284118).

---

## 1. Sample

- **175** late-type galaxies with `*_rotmod.dat` mass models
- Columns: Rad (kpc), Vobs, errV, Vgas, Vdisk, Vbul, surface brightness
- Quality flag Q from Table 1: 1 = high, 2 = medium, 3 = low
- Parsed Q match: Q1 ≈ 99, Q2 ≈ 64, Q3 ≈ 12 (minor name-matching ambiguity)

Stellar mass-to-light: \(\Upsilon_{\mathrm{disk}}=\Upsilon_{\mathrm{bulge}}=0.5\) at [3.6] (common RAR choice).

---

## 2. Locked disk law

\[
a_T = 8.25\times 10^{-11}\,\mathrm{m\,s^{-2}}
\]

Simple interpolator (no per-galaxy free parameters):

\[
g = \frac{g_N}{2} + \sqrt{\left(\frac{g_N}{2}\right)^2 + g_N a_T},
\qquad
g_N = \frac{V_{\mathrm{bar}}^2}{r},
\quad
V_{\mathrm{bar}}^2 = V_{\mathrm{gas}}^2 + \Upsilon_d V_{\mathrm{disk}}^2 + \Upsilon_b V_{\mathrm{bul}}^2.
\]

Score: mean absolute error (MAE) in km/s on \(V\) vs \(V_{\mathrm{obs}}\).

---

## 3. Results (median MAE)

| Sample | N | MAE \(a_T\) | MAE outer half | MAE Newtonian baryons only |
|---|---|---|---|---|
| All | 175 | 10.8 km/s | 10.3 | 38.2 |
| Q = 1 | 99 | 11.2 | 10.4 | 44.5 |
| Q = 2 | 64 | 9.7 | 8.5 | 26.8 |
| Q = 3 | 12 | 22.2 | 26.2 | 12.7 |

**Interpretation:** On Q = 1–2, the frozen one-constant law beats baryons-only by a wide margin (median ~11 km/s vs ~30–45 km/s). Q = 3 is small and low-quality; not used for claims.

---

## 4. Examples (Q = 1)

**Best MAE:** F583-4 (~1.4), DDO064 (~2.1), UGCA442 (~3.1), UGC07151 (~3.1)

**Worst MAE:** UGC02487 (~86), NGC5985 (~82), NGC2841 (~75) — typically massive systems where a single global \(\Upsilon\) and a simple interpolator struggle in the inner disk.

---

## 5. Relation to the locked floor

- No per-galaxy dark-halo parameters.
- One acceleration scale, same as Paper 1 product / DM floor notes.
- This is **exploration**, not a published SPARC fit: systematics (\(\Upsilon\), beam smearing, Q matching) remain.

---

## 6. Natural next steps on this data

1. Outer-only points with \(g_N < a_T\) (deep regime) and BTFR check.
2. Hold-out: train nothing (already zero free params) — report Q = 1 vs Q = 2 separately as here.
3. Compare \(a_T = 8.25\times 10^{-11}\) vs standard MOND \(a_0 \approx 1.2\times 10^{-10}\) on the same MAE.
4. Optional gas/helium factor from the papers if documented numerically.

---

## 7. Compact takeaway

SPARC is the right arena for the DM floor. A single frozen \(a_T\) already reduces typical velocity error by a factor of ~3–4 versus Newtonian baryons alone on quality 1–2 galaxies. Inner high-mass systems remain the hard cases.

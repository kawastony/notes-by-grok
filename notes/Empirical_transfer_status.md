# Empirical track — status (updated)

Tony Kawas / 14 September 2026.

---

## 1. SPARC full sample (locked protocol) — reconfirmed

| Quantity | Value |
|---|---|
| \(\Upsilon_{\mathrm{disk}}\) | 0.5 |
| \(\Upsilon_{\mathrm{bul}}\) | 0.7 |
| \(a_T\) | \(8.25\times 10^{-11}\,\mathrm{m\,s^{-2}}\) |
| Interpolator | Simple |
| Data | Rotmod_LTG (Zenodo 16284118 / CWRU) |

| Model | Median MAE (km/s) |
|---|---|
| Newtonian | **37.41** |
| TAFA | **10.82** |
| Improvement | **3.46×** |

No retuning.

---

## 2. THINGS-overlap subset (weak external-style split)

SPARC includes galaxies that are classic THINGS targets. Under the **same freeze**, a 13-galaxy THINGS-like subset:

| Galaxy | TAFA MAE | Newton MAE |
|---|---|---|
| NGC2403 | 10.82 | 44.90 |
| NGC2841 | 65.76 | 126.52 |
| NGC2903 | 17.37 | 51.37 |
| NGC2976 | 3.04 | 12.44 |
| NGC3198 | 7.02 | 50.50 |
| NGC3521 | 7.12 | 29.04 |
| NGC5055 | 17.33 | 42.28 |
| NGC6946 | 6.98 | 38.09 |
| NGC7331 | 16.59 | 51.55 |
| NGC7793 | 5.38 | 22.92 |
| IC2574 | 8.62 | 21.84 |
| DDO154 | 1.87 | 22.17 |
| NGC2366 | 6.69 | 17.25 |

| Aggregate | Value |
|---|---|
| Median TAFA MAE | **7.12 km/s** |
| Median Newton MAE | **38.09 km/s** |
| Improvement | **~5.3×** |

**Caveat:** These use **SPARC’s** mass models (Lelli pipeline), not independent de Blok/Oh radial \(V_{\mathrm{gas}},V_{\mathrm{disk}},V_{\mathrm{bul}}\) tables. So this is a **subset consistency** check, not a fully independent external transfer.

---

## 3. Fully independent THINGS / LITTLE THINGS \(V_{\mathrm{bar}}\)

| Source | Status |
|---|---|
| CDS VizieR Oh+2015 / de Blok+2008 mass-model tables | Still blocked or incomplete from this environment |
| Zenodo SPARC archive | Available (used above) |
| Requirement | Radial baryonic decomposition columns |

\[
\boxed{\text{True independent external }V_{\mathrm{bar}}\text{ transfer: still pending data access.}}
\]

---

## 4. Links used (user import)

- SPARC CWRU: https://astroweb.case.edu/SPARC/ (and cwru.edu mirror)
- Zenodo SPARC: https://zenodo.org/records/16284118
- VizieR J/AJ/152/157 (SPARC tables)
- arXiv 0810.2100 (THINGS paper; tables not fully ingested here)

---

## One-sentence close

Locked SPARC package holds (10.82 vs 37.41 km/s); THINGS-overlap galaxies under the same freeze give median TAFA MAE ~7.1 km/s (~5× vs Newton) as a subset check; fully independent THINGS/LITTLE THINGS baryonic decompositions remain the open empirical door.

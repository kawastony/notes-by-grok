# External / held-out disk tests

Tony Kawas / 10 September 2026. Item 2 of the three-step freeze.

Locked law only: \(a_T=8.25\times10^{-11}\), simple interpolator, \(\Upsilon_d=\Upsilon_b=0.5\). **Zero free parameters per galaxy.**

Data: SPARC Rotmod (Lelli+2016); unified corpus v3 for LITTLE THINGS kinematics (Flynn 2026 / Oh+2015 underlying).

---

## 1. SPARC Q=1 held-out split

Deterministic split by MD5(name): 40% holdout, 60% train (train not used to fit — law is frozen).

| Sample | N | med MAE \(a_T\) | mean MAE \(a_T\) | med Newton |
|---|---|---|---|---|
| Q1 train | 53 | 12.16 | 17.57 | 46.01 |
| **Q1 hold** | **46** | **10.57** | **15.82** | **42.87** |
| Q1 all | 99 | 11.24 | 16.76 | 44.50 |
| Q2 | 64 | 9.73 | 12.03 | 26.75 |

**Holdout is not worse than train.** Frozen floor generalises inside SPARC Q=1.

---

## 2. SPARC Q=1 dwarf proxy (\(V_{\max}<80\,\mathrm{km/s}\))

Stand-in for LITTLE THINGS–like systems while full Oh mass models are unavailable:

| Sample | N | med MAE \(a_T\) | med Newton |
|---|---|---|---|
| Q1 dwarfs | 19 | **5.47** | 25.95 |

Dwarfs are **better** fit under the same locked law (deep-MOND regime).

---

## 3. LITTLE THINGS (Oh+2015) via public corpus

| Fact | Value |
|---|---|
| Galaxies | 26 |
| Points | 1716 |
| Median \(V_{\max}\) | ~45 km/s |
| Median \(R_{\max}\) | ~3.4 kpc |
| \(V_{\mathrm{gas}}, V_{\mathrm{disk}}\) in corpus | **Absent** |
| SPARC name overlap | **0** in this naming |

**Limitation:** without baryonic decomposition, the frozen \(a_T\) law cannot be scored as MAE on \(V\) the way SPARC can. Kinematics-only confirms the sample is dwarf/irregular and outer-HI dominated — the regime where SPARC dwarfs already show med MAE ~5.5 km/s.

**Next data step (when available):** Oh+2015 mass-model tables with stellar+gas contributions → same MAE pipeline as SPARC.

---

## 4. Compact verdict

- Held-out SPARC Q=1: **pass** (med ~10.6 km/s, >> Newton).
- Dwarf proxy: **pass** (med ~5.5 km/s).
- LITTLE THINGS full MOND test: **blocked by missing \(V_{\mathrm{bar}}\)** in the public kinematics corpus used here; not a failure of the law.

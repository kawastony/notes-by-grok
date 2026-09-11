# Form-level discriminator — Simple μ vs RAR-favored forms

Tony Kawas / 11 September 2026. Layer C. Not Newton. Not generic MOND.

Protocol: Rotmod, Υ_disk=0.5, Υ_bul=0.7. N_points=3355, N_gal=175.

Forms:
- **Simple μ** (TAFA forced): \(g=\tfrac12 g_N+\sqrt{(\tfrac12 g_N)^2+g_N a}\)
- **Standard μ**: \(\mu=x/\sqrt{1+x^2}\)
- **Empirical RAR** (McGaugh): \(g=g_N/(1-e^{-\sqrt{g_N/a}})\)

Scales: \(a_T=8.25\times10^{-11}\), \(a_0=1.2\times10^{-10}\) m s^{-2}.

---

## RAR residual structure (log10 g_obs/g_pred)

| Form | med | rms | med\|log\| |
|---|---|---|---|
| Simple + a_T (**TAFA**) | +0.033 | 0.184 | 0.095 |
| Simple + a_0 | −0.020 | 0.185 | 0.091 |
| Standard + a_0 | +0.047 | 0.189 | 0.104 |
| Standard + a_T | +0.106 | 0.207 | 0.135 |
| **Emp RAR + a_0** | **−0.013** | **0.185** | **0.093** |
| Emp RAR + a_T | +0.040 | 0.185 | 0.097 |

---

## Per-galaxy median \|ΔV\| (km/s)

| Form | med MAE |
|---|---|
| Emp RAR + a_0 | **10.3** |
| Simple + a_0 | 10.4 |
| Simple + a_T | 10.7 |
| Emp RAR + a_T | 10.7 |
| Standard + a_0 | 10.8 |
| Standard + a_T | 13.2 |
| Newton | 38.5 |

Galaxy wins (Simple a_T vs Emp RAR a_0): **91 vs 84** — near coin-flip.

---

## Outer V (BTFR-like) log residual

| Form | med log10(V_obs/V_pred) | rms |
|---|---|---|
| Simple + a_T | +0.010 | 0.086 |
| Standard + a_0 | +0.005 | 0.087 |
| Emp RAR + a_0 | −0.021 | 0.090 |
| Simple + a_0 | −0.023 | 0.090 |

---

## Verdict (form-level, honest)

| Question | Answer |
|---|---|
| Does forced Simple+a_T beat Newton? | Yes (already known) |
| Does forced Simple+a_T beat Emp RAR+a_0? | **No clear win** — Emp RAR+a_0 slightly tighter on med MAE and RAR med bias |
| Does forced Simple beat Standard? | Yes on this sample (Standard+a_T notably worse) |
| Does SPARC prefer TAFA’s forced form over the empirically favored RAR form? | **Not significantly** — residuals compatible within the noise |
| Null-by-construction trap avoided? | Yes — comparison is form vs form, not MOND vs Newton |

**Reading:** SPARC does not reward the forced Simple+a_T form over the incumbent empirical RAR form. The form-level claim is **not empirically preferred** on this dataset; it is **not ruled out** either (91–84 galaxy split, rms nearly identical).

This is a high-value result: the data do not currently pay for the internal uniqueness argument at the form level.

---

## What this does *not* say

- That TAFA is wrong.
- That Simple μ is excluded.
- That internal package uniqueness is worthless (it remains a structural claim).
- That a_T is preferred over a_0 (still near-degenerate).

---

## Parallel priority (unchanged)

Define **pause-only** operationally: observable, sign/amplitude, competing predictions, dataset. Highest-ceiling ontology-level discriminator, not yet executable.

Clusters / high-z: still lower-clarity first moves.

---

## One-sentence close

On SPARC, the forced Simple-μ + a_T law fits well but does **not** outperform the empirically favored RAR form; the form-level discriminator is essentially a draw, so the uniqueness argument remains internal, not yet data-selected.

# Empirical track — status

Tony Kawas / 13 September 2026.

---

## 1. SPARC re-run (locked protocol)

Pre-commit unchanged:

| Quantity | Value |
|---|---|
| \(\Upsilon_{\mathrm{disk}}\) | 0.5 |
| \(\Upsilon_{\mathrm{bul}}\) | 0.7 |
| \(a_T\) | \(8.25\times 10^{-11}\,\mathrm{m\,s^{-2}}\) |
| Interpolator | Simple \(g=\tfrac12 g_N+\sqrt{(\tfrac12 g_N)^2+g_N a_T}\) |
| Metric | Median of per-galaxy mean \(|V_{\mathrm{obs}}-V_{\mathrm{model}}|\) |

**Result (175 galaxies, Rotmod_LTG):**

| Model | Median MAE (km/s) | Mean MAE |
|---|---|---|
| Newtonian | **37.41** | 39.93 |
| TAFA simple + frozen \(a_T\) | **10.82** | 14.91 |
| Improvement | **3.46×** | — |

Matches prior Empirical_protocol note. **Baseline SPARC package holds.**

---

## 2. True external transfer (THINGS / LITTLE THINGS)

### Requirement
Same protocol needs radial **baryonic decomposition**:
\[
V_{\mathrm{gas}}(r),\ V_{\mathrm{disk}}(r),\ V_{\mathrm{bul}}(r)
\]
not only \(V_{\mathrm{rot}}(r)\).

### What was attempted
| Source | Outcome |
|---|---|
| CDS/VizieR `J/AJ/149/180` (LITTLE THINGS) | Blocked (401 / bot challenge) |
| CDS `J/AJ/136/2648` (THINGS) | Not retrieved |
| Zenodo unified corpus | Gateway timeout / HTML |
| GitHub mirrors | No raw flat table with full \(V_{\mathrm{bar}}\) in reachable form |

Published THINGS/LITTLE THINGS **rotation** tables are widely available; **professional mass-model columns** matching SPARC’s Rotmod layout are not in this environment’s reachable downloads.

### Honest status
\[
\boxed{\text{External full-}V_{\mathrm{bar}}\text{ transfer: not completed (data access), not failed scientifically.}}
\]

No retuning was done. No claim of external MAE is filed.

---

## 3. Protocol for local completion

When machine-readable decompositions are available:

1. Freeze \(\Upsilon_{\mathrm{disk}}=0.5\), \(\Upsilon_{\mathrm{bul}}=0.7\), \(a_T\), simple interpolator.  
2. Build \(g_N=V_{\mathrm{bar}}^2/R\) with \(V_{\mathrm{disk}}\to V_{\mathrm{disk}}\sqrt{\Upsilon}\).  
3. Apply simple interpolator → \(V_{\mathrm{model}}\).  
4. Report median per-galaxy MAE vs Newtonian.  
5. **No** post-hoc \(\Upsilon\) or \(a_T\) change.  
6. File success **or** failure honestly.

---

## 4. What counts as empirical success

| Outcome | Meaning |
|---|---|
| External median MAE ≪ Newtonian, same order as SPARC ~10–15 km/s | Transfer **supports** package |
| External MAE near Newtonian | Package **does not** transfer under freeze |
| Only \(V_{\mathrm{rot}}\) available | Test **invalid** for this protocol (missing baryons) |

---

## One-sentence close

SPARC locked-protocol result is reconfirmed (median MAE 10.82 vs 37.41 km/s); true external transfer on THINGS/LITTLE THINGS awaits accessible full baryonic radial decompositions and is not claimed in either direction until then.

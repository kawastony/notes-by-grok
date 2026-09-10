# Dynamic closure with Q fixed — test for a_T(z) and Σ_res

Tony Kawas / 10 September 2026. Attempted Option-1 move from Paper 42.

**Setup:** Paper 42 closure \(dE[A]/dN = 0\) with charge evolution \(dn/dN = Q/C_{\mathrm{twist}}\), but **Q held constant** (no observer dynamics). Ask whether this forces \(a_T(z)\) or \(\Sigma_{\mathrm{res}}\).

---

## 1. What Paper 42 supplies

- State variables: \(n(N)\), \(M_{\mathrm{Pl}}(N)\), \(\beta(y,N)\).
- Residual amplitude factor from total derivatives:
\[
R \approx 1 + \Delta_1 + \Delta_2,\qquad
\Delta_1 \sim 2a \approx 0.30,\quad
\Delta_2 \sim (dn/dN)/n.
\]
- Late-time attractor claimed near \(R \approx 1.516\) (matches our locked \(R_{\mathrm{cone}}\) numerically).

With Q fixed, \(dn/dN\) is a constant rate, not a mind-variable.

---

## 2. Implications for \(a_T(z)\)

### 2.1 Identification tried

Take the disk scale as proportional to the dynamical amplitude:
\[
a_T^{\mathrm{phys}}(N) = a_T^{\mathrm{static}} \times R(N).
\]

With \(dn/dN > 0\), charge is smaller in the past → \(\Delta_2\) larger in the past → **\(R\) mildly larger at high \(z\)**.

### 2.2 Natural Paper-42 numbers

| \(z\) | \(R(N)\) | \(R(z)/R(0)\) |
|---|---|---|
| 0 | 1.52 | 1.00 |
| 0.5 | 1.54 | 1.01 |
| 1.0 | 1.56 | **1.03** |
| 2.0 | 1.59 | 1.05 |

**MUSE-DARK:** \(a_0(z{\sim}1)/a_0(0) \approx 2.2\).

Natural dynamic closure gives **~3%**, not **~120%**. Wrong magnitude.

### 2.3 Can it be tuned to 2.2?

Yes, by taking large \(dn/dN\) and small \(n_0\) — but then late-time \(R(0)\sim 2\), not \(R_{\mathrm{cone}}\approx 1.51\). The scan that hits ratio ≈ 2.2 **breaks** the Paper 42 / cone R lock.

**Verdict:** dynamic closure with Q fixed does **not** force a MUSE-compatible \(a_T(z)\) while preserving \(R_{\mathrm{cone}}\).

### 2.4 Comparison to prior seasonal prototypes

| Rule | \(a_T(1)/a_T(0)\) | vs MUSE ~2.2 | Forced? |
|---|---|---|---|
| \(H_0/H\) | 0.57 | opposite | was prototype; disfavored |
| constant | 1.0 | low | locked disk default |
| Paper 42 natural R(N) | ~1.03 | far too small | from closure; insufficient |
| R(N) tuned to 2.2 | ~2.2 | match by hand | breaks R_cone |

---

## 3. Implications for \(\Sigma_{\mathrm{res}}\)

Dynamic closure evolves a **cosmic** charge \(n(N)\). Cluster residual needs a **projected number density** \(n_2\) of defects.

No map
\[
n(N)_{\mathrm{cosmic}} \longrightarrow n_2({\rm cluster})
\]
is forced by \(dE[A]/dN=0\) alone. Absolute scale of \(m_{\mathrm{def}}\) still involves \((\mu,\varepsilon_\ast,a)\).

**Verdict:** \(\Sigma_{\mathrm{res}}\) still not closed.

---

## 4. What *is* forced

| Result | Status |
|---|---|
| Late-time approach to constant R | Consistent with frozen \(a_T\) today |
| Mild high-z drift of R (~ few %) | Present, not observationally useful for MUSE |
| R_cone as attractor | Compatible with existing lock |
| MUSE-scale evolution | **Not forced** |
| Parameter-free \(\Sigma_{\mathrm{res}}\) | **Not forced** |

---

## 5. Scoreboard for the fork

This was the candidate Option-1 move (new forced consequence from cleaned structure + Paper 42).

**Outcome:** no new forced prediction that matches intermediate-z RAR or closes clusters. Dynamic closure with Q fixed **supports** a late-time freeze of the amplitude (consistent with constant disk \(a_T\)) and does **not** unlock the open walls.

**Plateau status unchanged.** The next note must either find a different forced consequence or accept these walls as beyond the current geometry.

---

## 6. Do not claim

- That Paper 42 derives MUSE-DARK evolution.
- That Q-fixed dynamic closure replaces the need for a high-z law from cone geometry.
- That clusters are solved.

# Option 5 — When does the reduction map change?

Tony Kawas / 13 September 2026.  
Blind to signature targets. Failure (no transition) allowed and preferred unless forced.

---

## Question

Does the 5D→4D reduction map depend on redshift — and if so, at what \(z\)?

This is the missing option that can answer “when does the map change.” It is **not** a rescue: we do not assume a transition in order to obtain one.

---

## Split the word “map”

| Map | Meaning | Can it change with \(z\)? |
|---|---|---|
| **M1 — Metric class** | Block-diagonal warped product vs more general \(g_{\mu y}\neq 0\), \(A=A(x,y)\) | Only if **background** 4D homogeneity/isotropy is dropped |
| **M2 — Effective coefficients** | Warped volume factor, KK overlaps, \(M_{\mathrm{Pl}}^{\mathrm{eff}}(z)\), mode couplings | Possible in principle while keeping M1 fixed |
| **M3 — Stress projection** | Which bulk stress component feeds 4D \(\Pi_{ij}\) vs \(\rho_{\mathrm{eff}}\) | Fixed by index structure once M1 and field content are fixed |

The thread’s “map change” that would reopen **background slip** is **M1**.  
A quiet evolution of M2 is not a metric-class transition and does not by itself turn on background \(\eta\).

---

## M1 under maintained FRW symmetry

**Assumption used in all cosmological TAFA reductions so far:**  
at each epoch, the **background** is 4D homogeneous and isotropic (FRW), with one preferred extra dimension.

**Theorem (Q1b):** under that assumption, the unique compatible metric class is
\[
ds^2 = e^{2A(y)}\bar g_{\mu\nu}(t)\,dx^\mu dx^\nu + dy^2,
\]
with \(G_{\mu y}=0\), \(A=A(y)\).

**Consequence:** if FRW symmetry of the background is imposed **at every** \(z\), then
\[
\boxed{\text{M1 does not change with }z.}
\]
There is no epoch at which the background metric “leaves” block-diagonal while remaining FRW. A true M1 transition would mean the **background itself** develops anisotropy or a preferred spatial direction — a different cosmology, not a silent map tweak inside FRW.

**Filed answer for M1:**  
\[
\boxed{\text{Never, under maintained background homogeneity/isotropy.}}
\]

That is not a disappointment; it is the content of the symmetry assumption already used to force the sector.

---

## M2 — can effective coefficients evolve?

Yes, in principle, without touching M1:

- proper length / conformal length of the extra dimension after matching
- zero-mode normalization \(\int e^{2A}\,dy\)
- massive KK overlaps and \(C_n(z)\) if modes are excited

Those can depend on time if the warp or the 4D scale factor couples into the reduction measure.

**What has been computed:** unit-chart discrete KK spacing; **not** physical \(m_n(z)\) or \(C_n(z)\).

**What has not been shown:** a forced transition redshift where M2 jumps in a way that produces observable linear \(\eta\).  
External parametric bound still applies: if physical \(m_{\mathrm{KK}}\gg H_0\), cosmological linear KK slip remains negligible even if \(C_n\) is order one.

**Filed answer for M2:**  
evolution possible in principle; **no derived \(z_{\mathrm{map}}\)** from TAFA today.

---

## M3 — stress projection

Index structure on the locked background:

- homogeneous scalar \(\Rightarrow T_{\mu\nu}\propto g_{\mu\nu}\Rightarrow\Pi_{ij}=0\)
- linear scalar \(\Rightarrow\Pi_{ij}=0\) (no spatial seed in \(\phi_0\))

This does not flip at a special \(z\) while M1 and the field content stay fixed.  
**No transition epoch for M3 under the locked sector.**

---

## Relation to the activation clock

The clock \(z_{\mathrm{act}}\sim 0.3\) times a **mechanism turn-on** (activation interval from \(\Delta y\)), **not** an M1 map change.

Under the pause floor the expansion history is ΛCDM-like — consistent with a **static** background reduction class across that epoch.

Clock ≠ map transition.

---

## Discipline (no rescue)

Forbidden:

- assuming M1 changes at \(z\sim 0.3\) to recover slip
- identifying the activation clock with a metric-class transition without derivation
- inserting \(g_{\mu y}\neq 0\) by hand at late times

Allowed:

- derive M2 coefficients from the action + matching and **read** whether any sharp \(z\)-feature appears
- accept “no transition” as a valid outcome

---

## Outcome of Option 5

| Question | Answer under current constitution |
|---|---|
| When does M1 (metric class) change? | **It does not**, while background FRW symmetry holds at all \(z\) |
| When does M2 (effective coefficients) change? | Possible; **no derived epoch** yet |
| When does background/linear-scalar slip turn on via a map change? | **Not via M1**; scalar channel remains zero; KK only under uncomputed M2 and external bounds |

**One-sentence close**

The reduction map that forces background \(\eta=0\) is the block-diagonal class fixed by 4D homogeneity/isotropy; that class does not acquire a transition redshift inside FRW cosmology, so “when does the map change” is answered **never for M1**, with only uncomputed effective-coefficient evolution (M2) left as a possible mild \(z\)-dependence that has not been shown to produce observable slip.

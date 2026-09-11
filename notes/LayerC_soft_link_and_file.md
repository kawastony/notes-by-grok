# Soft-link audit — detailed balance pass — file decision

Tony Kawas / 11 September 2026. Layer C.

---

## Correction to prior note

**Do not say “minimality eliminated.”**

Accurate replacement:

> Bare aesthetic minimality was **replaced** by diluteness + single-scale / no-promotion logic. That is a real upgrade. It is **not** a full derivation of the global Simple μ shape. The transition region (\(x\sim 1\)) is where diluteness is weakest and where the interpolator’s shape is fixed — higher-order coefficients are not forced to zero there by diluteness alone.

### Split claims

| Claim | Status |
|---|---|
| **A.** Deep-regime rate linearity (\(r\sim x\) as \(x\to 0\)) | **Materially strengthened** (dimensions + flux + dilute one-body processes) |
| **B.** Global Simple μ | **Still conditional** on detailed balance + single-scale completion through the transition |

---

## One pass: detailed balance from cone irreversibility?

### What would be needed

Derive
\[
\frac{f_a}{f_p}=\frac{k_a}{k_p}
\]
from the cone update rule (neighbor bond currents, lock/unlock), without importing equilibrium chemical kinetics.

### What the lattice actually gives

- Unlock: energy/current-driven, rate \(\propto\) delivered work (already used).
- Lock: pause when strain drops below freeze scale (waist).
- No built-in requirement that forward and reverse rates satisfy **local detailed balance** at every site. A driven lattice can sit in a **nonequilibrium steady state** with cycles.

### Attempted closures (all soft)

1. **Assume near-equilibrium:** strain evolves slowly vs microscopic rates → approximate detailed balance. *Extra adiabatic assumption.*
2. **Entropy production minimisation:** linear IR response recovers Onsager symmetry → detailed balance in the linear regime only. *Does not fix nonlinear global μ.*
3. **Unique stationary distribution on two states:** two-state Markov chain with constant rates has the balance form by algebra — but that **assumes** a two-state Markov model, which is the kinetics package again.

### Verdict on this pass

| Goal | Result |
|---|---|
| Detailed balance derived from cone action / update rule alone | **No** |
| Detailed balance natural in linear near-equilibrium limit | Yes (standard) |
| Soft spot removed | **No** — moved into “near-equilibrium two-state kinetics” |

Per the stop rule written earlier: **do not recurse.** File the μ-shape result honestly and shift budget.

---

## Filed result (μ shape)

**Package-unique under stated assumptions:**

- two-channel (waist ontology)
- flux on active only
- single scale \(a_T\) with dimensional deep regime
- dilute one-body activation at small drive
- detailed balance (kinetics assumption — **named, not derived**)
- single-scale completion through transition

**Forced:** deep-regime linearity of the rate ratio.  
**Conditional:** global Simple interpolator.  
**Not claimed:** pure cone-Lagrangian theorem; SPARC discrimination vs \(a_0\).

---

## Budget shift (stop rule applied)

| Item | Action |
|---|---|
| Further pure-kinetics recursion on detailed balance | **Stopped** |
| μ shape status | **Filed** as package-unique / conditional global |
| Empirical discrimination \(a_T\) vs \(a_0\) | **Active** |
| Derive \(a_T\) | Long-game, parallel if cheap |

Internal elegance does **not** replace external discrimination. SPARC MAE near-degeneracy remains the empirical fact.

---

## Standing Layer C scoreboard (honest)

| Element | Status |
|---|---|
| SPARC fit quality | Real (~10.7 vs Newton 38.5 km/s) |
| μ shape | Package-unique under named assumptions; deep linearity strengthened |
| Detailed balance | Soft link — filed |
| \(a_T\) vs \(a_0\) | Empirically near-degenerate on SPARC |
| Scale derivation | Open |
| Distinctive non-galaxy prediction | Open — highest remaining external value |

---

## One-sentence close

Deep-regime linearity is on firmer ground; global Simple μ is still conditional on kinetics assumptions we did not derive; minimality was improved into diluteness but not erased; recursion on detailed balance stops here; the next decision-relevant work is empirical discrimination or a pause-only / high-z / cluster observable, not another internal purity loop.

# Activation soft spot — Paper 13 tunneling vs linear rate; golden bridge

Tony Kawas / 10 September 2026. Attempt to close energy-driven activation; glean from papers.

---

## Question

Is activation on the cone lattice **necessarily** energy-driven (rate ∝ bond work ∝ g), or are other geometric laws allowed?

---

## Three laws on the same lattice

| Law | Rule | Continuum μ shape | φ at transition? |
|---|---|---|---|
| Hard threshold | unlock iff \(|\nabla\varepsilon|>\delta_\ast\) | step / soft step | **No** |
| Linear energy-driven | \(k_a\propto\) bond work \(\propto g\) | \(x/(1+x)\) | **Yes** |
| Euclidean tunneling (Paper 13) | rate \(\propto e^{-S_{\mathrm{cone}}}\) | Arrhenius / barrier-dependent | **Not automatically** |

---

## What Paper 13 actually supplies

Two-sector cone; activation as **topological interpolation** between sectors; Euclidean junction action \(S_{\mathrm{cone}}\) from tension + mismatch barrier. Own caveat: not a complete first-principles mass derivation.

Implications for rates:

- Barrier independent of local \(g\) → constant attempt rate (not linear).
- Barrier lowered by work, \(S=S_0-\alpha(g/a_T)\) → rate \(\propto\exp(\alpha g/a_T)\) (**exponential**, not linear).
- Linear rate can appear only as a **local expansion** of a smoother law, not as the tunneling law itself.

So Paper 13 is a **geometric alternative** from the same ontology that does **not** force \(k_a/k_p=g/a_T\).

---

## Golden bridge

Investigated (Golden_bridge_and_10D_QG.md, Papers 38/42/44 lineage).

- Role was UV-parent naming and parking \(11/72\), \(R\) in a 10D dictionary.
- That bookkeeping was already **retired** (not derived from 5D action; replaced by cone accounting).
- No microscopic disk activation rule for \(\mu(g)\) is stated there.

**Not applicable** to this soft spot.

---

## Verdict

| Claim | Result |
|---|---|
| Soft spot closed (energy-driven necessary) | **No** |
| Hard threshold ruled out for φ | **Yes** |
| Linear energy-driven sufficient for simple μ | **Yes** |
| Linear energy-driven necessary | **No** — Paper 13 tunneling is allowed |
| Golden bridge helps | **No** |

**Status of Prediction B package:**

> Simple interpolator follows from two-channel + flux-on-active + **linear** detailed balance. Linearity is sufficient and natural, but Paper 13 shows a cone-native alternative (tunneling) that does not yield the same μ. The gap is not closed; if anything it is better mapped: the competing geometric law is tunneling, not a generic free function.

---

## Do not

- Claim the interpolator is now a pure cone theorem.
- Use golden-bridge dictionary numbers as microscopic rates.
- Promote Prediction A.

## Possible next (only if still pursuing this gap)

Coarse-grain a dilute gas of Paper 13–style cone-junction instantons in a background strain \(\propto g\) and compute the effective unlock rate. If that calculation returns a leading term linear in \(g\), linearity becomes a theorem of the instanton gas; if it returns exponential, simple μ is disfavored by the same geometry that was meant to support it.

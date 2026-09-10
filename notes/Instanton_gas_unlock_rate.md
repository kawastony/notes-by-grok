# Instanton gas coarse-grain — unlock rate vs simple μ

Tony Kawas / 10 September 2026. Paper 13–style junction instantons in background strain.

---

## Setup

Dilute gas of cone-junction Euclidean events. Rate per locked site:
\[
k(s)=\Gamma(s)\,e^{-S(s)},\qquad s=|\nabla\varepsilon|/\delta_\ast\propto g/a_T.
\]

---

## Barrier models and resulting μ

| Model | \(S(s)\) / prefactor | \(k(s)\) | Effective \(\mu\) | φ? |
|---|---|---|---|---|
| T1 pure topological | \(S=S_0\) | const | saturates | No |
| T2 strain-biased barrier | \(S=S_0-\beta s\) | \(\propto e^{\beta s}\) | logistic \(1/(1+C e^{-\beta x})\) | No (height depends on β,C) |
| T3 soft quadratic | \(S=S_0-\beta s+\gamma s^2/2\) | exp of quadratic | not \(x/(1+x)\) | No |
| T4 linear prefactor | \(S=S_0\), \(\Gamma\propto s\) | \(\propto s\) | \(x/(x+c)\) | Yes if \(c=1\) |
| T5 classical over-barrier | high-\(s\) | \(\propto s\) | linear-channel | Yes in that regime |

Numerical (T2): at parameters tried, the \(x\) solving \(\mu(x)\,x=1\) lies ~1.06–1.45, **not** φ≈1.618.

---

## What Paper 13 favors

Native object is a **large topological exponent** \(S_{\mathrm{cone}}\sim 60\!-\!70\) from junction tension + mismatch. Strain coupling is not derived there → closer to **T1/T2**, not T4.

T4 recovers simple μ only by putting linearity into the **attempt frequency**. That is the same soft spot under another name.

---

## Verdict

| Claim | Result |
|---|---|
| Instanton gas ⇒ \(k_a/k_p=g/a_T\) as theorem | **Fails** |
| Tunneling alone ⇒ simple μ / φ | **Fails** (logistic μ; height not φ) |
| Linear prefactor or classical channel needed for simple μ | **Yes** — reintroduces the soft spot |
| Soft spot closed | **No** |

**Stronger negative result than before:** the most cone-native activation law from Paper 13 (Euclidean junction tunneling) **does not** produce the simple interpolator. Getting simple μ still requires an extra linear channel (prefactor or over-barrier classical).

---

## Scoreboard impact

Prediction B package remains:

> simple interpolator = forced **under linear detailed balance**; linear balance = **not** forced by Paper 13 tunneling geometry.

Do not promote B to derivation test. Do not promote Prediction A.

---

## Recommended posture

This line (close the rate gap via discrete rule / instantons) has been driven to a clear negative: **tunneling gas ≠ simple μ**. Further iterations of the same gap without a new principle are ledger work.

Honest options:

1. **Accept the gap** — keep simple μ as motivated by linear two-channel balance; label B conditional; move to a different forced prediction.
2. **Compute a full instanton-gas μ(x)** with a *specified* strain coupling from the cone metric (not a free β) and accept whatever shape appears — even if it is not simple.
3. **Drop simple μ** as the preferred interpolator and let the cone dictate a different response function from (2).

Option 1 is the plateau-preserving move. Options 2–3 are the only ways this activation thread can still produce new geometry-driven content.

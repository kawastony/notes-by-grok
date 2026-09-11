# Constitutive transport — floor vs average, k and z structure

Tony Kawas / 11 September 2026. Layer C. Time-boxed attack on α_c and the slip kernel.

Addresses critique: is 1/3 a **hard geometric floor** or an **orientation average**? Name volume-preservation as package assumption. Sketch k,z structure without a full Boltzmann code.

---

## 1. Package assumptions (visible)

| Assumption | Status |
|---|---|
| Volume constraint \(R^2L=\mathrm{Vol}_0\) | Locked algebra |
| Pause branch \(N=0\) | Locked ontology |
| Residual size \(\varepsilon_{\mathrm{res}}\sim11/72\) | Locked accounting |
| Residual of a volume-preserving deformation is traceless | **Package assumption** — natural, not independently derived from a 4D effective action |
| Quasi-static sub-horizon slip responds to anisotropic stress at O(1) | Standard GR reading |

Volume-preservation → traceless is **not** optional rhetoric; it is an active assumption of the constitutive map. If residual freeze were allowed a trace part, the hide-in-Λ route reopens.

---

## 2. Traceless residual → anisotropic stress (solid)

With the volume-preserving assumption:
\[
\mathrm{tr}\,\varepsilon_{\mathrm{res}}=0
\quad\Rightarrow\quad
\text{residual cannot be pure }\delta\rho\text{ in the effective fluid.}
\]

The residual stress has a **traceless** piece. In the cosmological effective fluid that piece is anisotropic stress \(\sigma\). That closes the pure-Λ escape. **This part stands.**

---

## 3. The 1/3 is an orientation average, not a hard floor

### What random-orientation averaging gives

Local residual elongation: uniaxial traceless strain along a cone axis \(\hat n\).

Stress contribution schematically:
\[
\Pi_{ij}\;\propto\;\varepsilon_{\mathrm{res}}\Bigl(\hat n_i\hat n_j-\tfrac13\delta_{ij}\Bigr).
\]

Sky / network average for **uncorrelated** random \(\hat n\):
\[
\langle\Pi_{ij}\rangle = 0.
\]

The **mean** anisotropic stress vanishes. What survives in the scalar sector of cosmological perturbation theory is the **variance** projected onto the longitudinal scalar anisotropic stress, or any **net alignment** residual.

**Standard result for randomly oriented uniaxial inclusions:** the effective scalar anisotropic-stress amplitude that sources \(\Phi-\Psi\) is suppressed by a geometric factor of order
\[
\frac{1}{3}\quad\text{to}\quad\frac{2}{5}
\]
relative to the fully aligned case — this is an **average / RMS projection factor**, not a theorem that every configuration satisfies \(|\sigma|\ge\varepsilon_{\mathrm{res}}/3\).

### Hard lower bound?

**No.** Volume preservation forbids pure trace; it does **not** forbid:

- nearly isotropic *networks* whose orientation-averaged \(\Pi_{ij}\) is tiny;
- cancellations between regions;
- residual mostly in vector/tensor sectors that average out of the scalar slip.

So:

| Statement | Status |
|---|---|
| Residual is traceless locally | Forced under volume-preserving assumption |
| Typical / random-orientation scalar projection \(\sim1/3\) | **Motivated average** |
| Strict floor \(|\eta|\ge0.05\) for all allowed configs | **Not derived** |
| Escape to \(\alpha_c\ll1/3\) via isotropy of the *network* | Still open |

**Correction to prior note:** replace “hard floor 1/3” with “**typical orientation average \(\sim1/3\)**.” The band becomes:

\[
|\eta|_{z\,\lesssim\,0.3}\;\sim\;\alpha_c\,\frac{11}{72},
\qquad
\alpha_c\;\in\;(0,1],
\]
with **expected** \(\alpha_c\sim1/3\) for random networks and \(\alpha_c\sim1\) for coherent alignment. The pure-Λ escape (\(\alpha_c=0\) by dumping residual into trace) remains closed; a **network-isotropy** escape remains open.

---

## 4. k and z structure of the slip (sketch)

### z structure (sharp claim, retained)

\[
|\eta|(z)\;\approx\;
\begin{cases}
\sim0 & z\gg z_{\mathrm{tr}}\sim0.3\quad(\text{pre-freeze})\\
\alpha_c\,\varepsilon_{\mathrm{res}} & z\lesssim z_{\mathrm{tr}}\quad(\text{pause residual on})
\end{cases}
\]

Turn-on near the activation interval is still the **sharpest** discriminator. High-z nulls remain consistency checks.

### k structure (quasi-static sketch)

In Newtonian gauge, scalar anisotropic stress enters schematically:
\[
\Phi-\Psi \;=\; -12\pi G a^2\,(\bar\rho+\bar P)\,\sigma\,/\,k^2
\quad\text{(convention-dependent coefficient).}
\]

For a residual stress that is **not** free-streaming radiation but a quasi-static network residual, \(\sigma\) itself may be only weakly k-dependent on sub-horizon scales. Then:

- **Large scales (small k):** slip can approach a constant plateau set by \(\alpha_c\varepsilon_{\mathrm{res}}\).
- **Deep sub-horizon:** same plateau if \(\sigma\) is scale-independent; if residual is correlated only below a network scale \(\lambda_{\mathrm{net}}\), slip cuts off for \(k\gg 1/\lambda_{\mathrm{net}}\).

Without a derived network scale, the default working assumption is **scale-independent late-time slip below the horizon**, amplitude \(\alpha_c\times11/72\), turned on for \(z\lesssim0.3\).

That is enough to specify a **step-binned, scale-independent η template** for comparison with Stage-III/IV analyses — the fair empirical target.

---

## 5. Updated empirical reading

Against \(\Sigma_0=0.008\pm0.045\) (smooth template):

| \(\alpha_c\) | \(|\eta|\) | Indicative pressure |
|---|---|---|
| 1 (aligned) | ~0.15 | Strong |
| ~1/3 (random avg) | ~0.05 | Mild / marginal |
| ≪1/3 (network near-isotropic) | ≪0.05 | Weak — **still allowed**; no longer forbidden by a hard floor |

**Honest status:**

- Pure-Λ hide closed.
- Hard 1/3 floor **withdrawn**.
- Expected band still centered near 0.05–0.15.
- Model **survives** current indicative comparison most comfortably if the network is not fully aligned; **pressured** if aligned.
- Not directly tested until a **step at \(z\sim0.3\)** is fitted, not only smooth \(\Omega_{\mathrm{DE}}\) MG.

---

## 6. What would close the remaining soft joint

| Calculation | Pays off |
|---|---|
| Effective \(\langle\Pi_{ij}\rangle\) from an explicit cone-network ensemble | Fixes typical \(\alpha_c\) vs distribution |
| Match residual stress to scalar-vector-tensor decomposition | Shows how much leaks out of scalar slip |
| Step-binned η likelihood on DESI×lensing | Fair empirical test of turn-on |

Time-box: ensemble average of random cones is the next **cheap** theory step; full Boltzmann is not required to state the template.

---

## 7. Filed statements (corrected)

1. Residual is traceless under volume-preserving freeze → sources anisotropic stress, not pure Λ.  
2. **1/3 is an orientation average, not a hard floor.**  
3. Expected \(|\eta|\sim0.05\)–0.15 for \(z\lesssim0.3\); lower values possible if network averages toward isotropy.  
4. Sharp observable claim: **turn-on near \(z\sim0.3\)** at fixed ΛCDM \(H(z)\).  
5. GR / Simple-μ MOND+Λ: η≈0 always.

---

## One-sentence close

Volume preservation still closes the pure-Λ escape and keeps residual stress anisotropic locally, but the factor 1/3 is only a **typical orientation average**, not a configuration-wide floor; the slip prediction remains a late-time turn-on of amplitude **typically** \(\mathcal{O}(0.05\)–0.15)\), with network isotropy as the remaining low-amplitude escape, to be fixed by an ensemble average or by a step-binned empirical test.

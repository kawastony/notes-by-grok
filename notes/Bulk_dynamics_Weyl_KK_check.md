# Bulk dynamics — Weyl/KK check

Tony Kawas / 12 September 2026. Verify pasted claims; explore bulk graviton sector.

---

## 1. What the literature actually says

Projected bulk Weyl on the 4D slices (SMS and thick-warp analogues):
\[
E_{\mu\nu}\equiv C_{\mu A\nu B}\,n^A n^B
\]
decomposes as a Weyl fluid: dark radiation density \(\rho_E\), momentum \(q_E\), and anisotropic stress \(\pi^E_{\mu\nu}\).

| Setting | \(\pi^E\) / slip |
|---|---|
| Exact FRW **background** (maximal spatial symmetry) | \(\pi^E=0\) by symmetry — only isotropic dark radiation \(\rho_E\propto a^{-4}\) |
| **Linear perturbations** about FRW | \(\pi^E\) **need not vanish** — carries nonlocal KK/spin-2 content; no closed 4D evolution equation for \(\pi^E\) in general |
| Conformally flat bulk (pure AdS) unperturbed | \(E_{\mu\nu}=0\) |

**Correction to the pasted claim:**  
“Zero linear slip from bulk Weyl on FLRW” is true for the **background**. It is **not** a theorem for linear cosmological perturbations: that is exactly where braneworld theory leaves \(\pi^E\) as a free nonlocal source unless the bulk is solved.

So the ladder is:

| Sector | Linear cosmological slip |
|---|---|
| Background scalar + geometry | 0 (theorem) |
| Linear TAFA scalar | 0 (theorem) |
| 2nd-order scalar | \(\sim10^{-10}\) irrelevant |
| Background Weyl | 0 (symmetry) |
| **Linear Weyl / KK** | **Open unless bulk solved** |

---

## 2. Bulk dynamics sketch for TAFA’s warp

### Geometry from Open B

Unit-chart profiles: finite interval to the field-space wall, \(A_{\mathrm{end}}\sim-0.4\) (shallow), no exponential RS throat.

Extra-dimension proper length is O(1) in unit chart. After matching to a physical \(M_{\mathrm{Pl}}\), the KK scale is set by that length:
\[
m_{\mathrm{KK}}\sim \frac{1}{L_5^{\mathrm{phys}}}.
\]
Without a deep warp, there is **no automatic TeV hierarchy** and no automatic \((H_0/m_{\mathrm{KK}})^2\) suppression from an exponential throat. The physical \(L_5\) is not fixed until Open A / Planck matching is done — still open.

### Graviton KK problem (not solved here)

Tensor perturbations of the 5D metric, after gauge fixing and field redefinition, obey a Schrödinger-like equation in the conformal coordinate \(z\):
\[
-\frac{d^2\psi}{dz^2}+V_{\mathrm{eff}}(z)\psi=m^2\psi,
\qquad
V_{\mathrm{eff}}\sim (\partial_z A)^2+\partial_z^2 A
\]
(with the standard warped weight).

For TAFA’s shallow \(A(y)\):
- A normalizable **massless zero mode** is expected if the warp volume is finite (standard 4D graviton).
- Massive KK tower spacing ~ \(1/L_5\).
- Wavefunction overlap with the observable sector controls coupling.

Until this eigenvalue problem is solved with TAFA’s actual \(A(y)\) and boundary conditions at the tip/wall, one cannot claim either “no coupled mode” or “observable slip.”

### Parametric expectation (not a derivation)

If after matching \(m_{\mathrm{KK}}\gg H_0\) (true for any sub-mm extra dimension),
\[
\Phi-\Psi\sim\mathcal{O}\!\left(\frac{H^2}{m_{\mathrm{KK}}^2}\right)\times(\text{mode amplitude})
\]
is negligible in the cosmological regime. That is the usual reason KK gravity does not wreck solar-system or CMB tests when the compactification scale is high.

This is **parametric**, not a TAFA computation. Filing a number would require the spectrum + overlap + projection.

---

## 3. Check of pasted answers

| Pasted claim | Assessment |
|---|---|
| Background FRW ⇒ \(E_{ij}^{\mathrm{TF}}=0\) | **Correct** |
| Background Weyl ⇒ \(\eta=0\) | **Correct** |
| Linear Weyl ⇒ \(\eta=0\) automatically | **Too strong** — linear \(\pi^E\) is the open nonlocal piece |
| Slip needs anisotropic spin-2 KK that break isotropy | **Directionally correct** for the perturbation sector |
| Scalar + background Weyl close the freeze | **Yes** for those sectors |
| Linear KK/Weyl closed without bulk solve | **No** |

---

## 4. What “explore bulk dynamics” yields for the freeze

1. Reinforces: scalar channel and background Weyl give \(\eta=0\).
2. Clarifies: linear bulk gravity remains the only logical open door, and only at the level of an unsolved spectral problem.
3. Does **not** produce a derived \(|\eta|\). Shallow warp makes a deep-throat suppression story unavailable; high KK scale (if present after matching) would suppress slip parametrically — still not computed.

**Guardrail:** Do not promote KK slip as a TAFA prediction. Do not revive \(11/72\to\eta\) or \(\varepsilon\to\eta\).

---

## 5. Legitimate next step if bulk is pursued

Only this sequence, failure allowed:

1. Take numerical \(A(y)\) from Open B (physical units after Planck matching).
2. Form \(V_{\mathrm{eff}}(z)\); solve Sturm–Liouville for graviton modes with tip/wall BCs.
3. Read zero mode + mass gap + overlaps.
4. Project to \(\delta E_{ij}^{\mathrm{TF}}\) / \(\Pi_E\).
5. Evaluate cosmological \(\Phi-\Psi\) scaling — **last**.

If any step fails or is underdefined (matching, BCs), stop and leave KK unclaimed.

---

## One-sentence close

Background Weyl is isotropic (\(\eta=0\)) by FRW symmetry, and the TAFA scalar remains slip-silent through second order; linear bulk KK/Weyl anisotropic stress is a real open possibility in 5D Einstein gravity but is not derived for TAFA’s shallow warp and stays outside the frozen outward claim of mechanism + epoch.

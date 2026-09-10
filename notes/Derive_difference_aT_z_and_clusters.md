# Derive a difference: a_T(z) and cluster-scale cone

Tony Kawas / 10 September 2026. Response to the boat-compass: stop same-lake fitting; **build a seasonal / rapids rule from the theory**.

Not a paper. Attempts only what the existing spine forces or almost forces.

---

## A. Seasonal rule — candidates for a_T(z)

### A0. What is locked today

From Floor_DM:

\[
a_T = \Lambda_*^2 \mu = 8.25\times 10^{-11}\,\mathrm{m\,s^{-2}}
\]

**Calibrated**, not derived. Any \(a_T(z)\) must say how \(\Lambda_*\) or \(\mu\) runs with cosmic time **without** retuning on SPARC.

### A1. Coincidence route (not forced by TAFA)

\[
c H_0 \approx 6.8\times 10^{-10}\,\mathrm{m\,s^{-2}},
\qquad
\frac{a_T}{c H_0}\approx 0.12,
\qquad
\frac{a_0}{c H_0}\approx 0.18.
\]

If one **postulates** \(a_T(z)=a_T(0)\,E(z)\) with flat \(\Lambda\)CDM \(E(z)\):

| \(z\) | \(E\) | \(a_T(z)/a_T(0)\) |
|---|---|---|
| 0 | 1 | 1 |
| 0.5 | 1.31 | 1.31 |
| 1 | 1.76 | 1.76 |
| 2 | 2.97 | 2.97 |
| 6 | 10.2 | 10.2 |

**Status:** falsifiable with high-z rotation/lensing, but **not derived** from cone or 5D. It is the MOND “\(a\sim cH\)” slogan applied to \(a_T\). Do not claim it is TAFA until \(\Lambda_*\mu\propto H\) is forced.

### A2. 5D activation interval route (forced geometry, weak map to a_T)

Forced:

\[
\Delta y = 0.2445\,\frac{f}{\Lambda^2},
\qquad
\Delta g = -2\Delta y = -0.489
\quad(f=\Lambda=1).
\]

Paper-41 linear map gives a **late-time** redshift of order \(z\sim 0.3\) for O(1) drivers — the DE activation window, not a disk law.

**Proposed (honest, provisional) seasonal rule:**

1. Cosmic field freezes on the **pause branch** for \(z < z_{\mathrm{tr}}\) with \(z_{\mathrm{tr}}\sim 0.3\) from the activation interval.
2. Disk floor \(a_T\) is set by the frozen local slope of the cone after pause, hence **constant for \(z \lesssim z_{\mathrm{tr}}\)**.
3. For \(z \gg z_{\mathrm{tr}}\) the field is still rolling; the effective acceleration scale is **not** guaranteed to equal today's \(a_T\).

That yields a **step or soft step**, not a continuous \(E(z)\) law:

\[
a_T(z) \approx
\begin{cases}
a_T(0) & z \lesssim 0.3 \\
\text{undetermined without a roll→disk map} & z \gg 0.3
\end{cases}
\]

**What this predicts that MOND (constant \(a_0\)) does not:**
possible **deviation of the RAR zero-point at \(z\gtrsim 1\)** once a roll→disk map is written. Until that map exists, high-z tests cannot be scored — same gap as before, now named precisely.

**Missing closed step:** express local disk \(a_T\) as a functional of the bulk field after freeze (e.g. from wall residual pressure or \(\varepsilon_\ast\) magnitude). That is the real derivation, not this note.

### A3. Pause branch alone does not give a_T(z)

Volume constraint pause \(N=0\) freezes the **cosmological** field. It does not by itself change the **galactic** interpolator. Linking them is an extra identification (the “roll→disk map”).

---

## B. Rapids rule — cluster-scale cone sketch

### B1. Why disks work and clusters fail for pure a_T

Disks: ordered, thin, roughly isolated; one acceleration scale and simple interpolator suffice.

Clusters: multi-body, large external fields, hot gas + galaxies, mergers. MOND (and pure \(a_T\)) leave residual mass ~ \(M_{\mathrm{baryon}}\).

### B2. Cone-network ingredients already on the shelf

| Ingredient | Possible cluster role |
|---|---|
| Cone network / elongation transfer | Collective field; not single-particle DM |
| External field effect (EFE) | System in a larger cone background — reduces boost |
| Defect charge / residual pressure | Unresolved defects as **collisionless residual mass** |
| Waist / pause | Not a cluster fix |

### B3. Minimal distinguishing claim (provisional)

**Claim C1 (testable in principle):** residual cluster mass is **defect density** of the cone network, hence:

- traces **collisionless** structure (galaxies / subhalos), not the X-ray gas — same qualitative side as CDM on Bullet-like systems;
- amount set by network topology / coarse-graining scale, **not** by rescaling \(a_T\).

**Claim C2:** pure acceleration-scale MOND has no defect sector; TAFA does. That is the **logical** distinction. It is **not** yet a calculation of the residual mass fraction.

**Missing closed step:** write residual surface density

\[
\Sigma_{\mathrm{res}} \sim n_{\mathrm{def}}\,q_0\ \text{or}\ \varepsilon_\ast\text{-energy per area}
\]

and confront Bullet residual ~ few ×10^{14} M_⊙. Until numbers appear without free \(n_{\mathrm{def}}\), this is a program, not a pass.

### B4. What not to do

- Do not lower \(a_T\) further to “help” clusters (destroys disks).
- Do not add a free cluster-only scale.
- Do not call C1 proven.

---

## C. What was actually derived vs postulated

| Statement | Status |
|---|---|
| \(\Delta y\) and late-time activation window | Derived (5D) |
| \(a_T(z)=a_T(0)\,E(z)\) | Postulate (coincidence) |
| \(a_T\) constant for \(z\lesssim 0.3\) after pause | Plausible identification, not closed |
| Roll→disk map for high-z \(a_T\) | **Missing** |
| Defect residual mass in clusters | Logical option from network; **unquantified** |
| Residual mass number for Bullet | **Not derived** |

---

## D. Compass after this attempt

1. **Highest closed next equation:** roll→disk map
   \[
   a_T = F[\phi_{\mathrm{freeze}}, A_{\mathrm{wall}}, \varepsilon_\ast]
   \]
   so that high-z RAR becomes a real prediction.

2. **Second:** one formula for \(\Sigma_{\mathrm{res}}\) from defect density with no free cluster scale.

3. Until those exist, the boat still floats with MOND on disks and still sinks on cluster rapids.

**One sentence:** We named how a seasonal rule and a rapids rule *could* be forced by 5D pause and cone defects; we did not yet force the numbers — the next work is those two maps, not another SPARC lake.

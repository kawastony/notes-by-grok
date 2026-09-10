# Roll→disk map and Σ_res from defects

Tony Kawas / 10 September 2026. Attempted closed maps. Not a paper.

Goal: write
\[
a_T=F[\phi_{\mathrm{freeze}},A_{\mathrm{wall}},\varepsilon_\ast]
\]
and
\[
\Sigma_{\mathrm{res}}=G[\text{defect density, network scales}]
\]
with as little free structure as the spine allows.

---

## 1. Roll→disk map

### 1.1 Ingredients already on the shelf

| Object | Role |
|---|---|
| Pause branch \(N=0\) | field frozen; \(\dot\phi=0\) |
| Freeze on slope | \(V_A(\phi_{\mathrm{freeze}})=\rho_\Lambda\) (old solution; sky-degenerate with \(\Lambda_0\)) |
| Wall | \(\phi\to\pm\pi f\), \(A\to-1/2\) in 5D |
| \(\Delta y=0.2445\,f/\Lambda^2\) | late-time geometric tick \(z_{\mathrm{tr}}\sim 0.3\) |
| Network magnitude | \(\lvert\boldsymbol{\varepsilon}\rvert\to\varepsilon_\ast\) outside cores (Law 4 / condensate) |
| Locked product | \(a_T=\Lambda_*^2\mu=8.25\times10^{-11}\,\mathrm{m\,s^{-2}}\) (calibrated) |

### 1.2 Dimensional bridges (forced shapes, not forced coefficients)

Energy density of freeze: \(\rho_{\mathrm{fr}}=V_A(\phi_{\mathrm{freeze}})\).

Three acceleration-dimension combinations built only from \((\rho_{\mathrm{fr}},G,c)\):

\[
\begin{align}
a_{(1)}&=\sqrt{G\rho_{\mathrm{fr}}}\,c,\\
a_{(2)}&=G\rho_{\mathrm{fr}}R_H,\qquad R_H=c/H_0,\\
a_{(3)}&=cH_0.
\end{align}
\]

Numbers today (\(\rho_{\mathrm{fr}}=\rho_\Lambda\approx0.7\rho_c\), \(H_0=70\)):

| Combination | Value (m s^{-2}) | / \(a_T\) |
|---|---|---|
| \(a_{(1)}\) | \(1.97\times10^{-10}\) | **2.38** |
| \(a_{(2)}\) | \(5.68\times10^{-11}\) | **0.69** |
| \(a_{(3)}\) | \(6.80\times10^{-10}\) | **8.24** |
| locked \(a_T\) | \(8.25\times10^{-11}\) | 1 |

So **order-of-magnitude** the freeze density already knows \(a_T\) through cosmology. That is the same coincidence MOND uses (\(a_0\sim cH\)); it is **not yet** a derivation of the number 8.25×10^{-11}.

### 1.3 Proposed map (provisional closed form)

Identify the disk floor with the freeze density and the Hubble radius **after pause**:

\[
\boxed{
a_T(z)\;\equiv\;
\xi\,G\,\rho_{\mathrm{fr}}(z)\,R_H(z)
}
\]
with
\[
\rho_{\mathrm{fr}}(z)=V_A\bigl(\phi_{\mathrm{freeze}}(z)\bigr)
\]
and, on the pause branch for \(z\le z_{\mathrm{tr}}\),
\[
\phi_{\mathrm{freeze}}=\mathrm{const},\qquad
\rho_{\mathrm{fr}}=\rho_\Lambda,\qquad
R_H=c/H(z).
\]

**Coefficient \(\xi\):** matching today forces
\[
\xi=\frac{a_T}{G\rho_\Lambda R_H(0)}\approx 1.45.
\]

That is **one** dimensionless number from matching the locked product — not a free function, but not derived from wall geometry either.

**Wall / \(\varepsilon_\ast\) entry (optional tightening):**

If the preferred magnitude is set by the wall residual,
\[
\varepsilon_\ast^2\propto \frac{V_A(\phi_{\mathrm{near\ wall}})}{\mu c^2}\quad\text{(order of magnitude)},
\]
then \(\varepsilon_\ast\) tracks the same freeze energy and does not add a second independent scale to \(a_T\). It supports the map; it does not yet compute \(\xi\).

### 1.4 What the map predicts that constant-\(a_0\) MOND does not

On pause for \(z\le z_{\mathrm{tr}}\sim0.3\):
\[
a_T(z)=a_T(0)\,\frac{H(z)}{H_0}
\]
(because \(\rho_{\mathrm{fr}}\) fixed and \(R_H\propto1/H\) cancels one power — wait:

Careful:
\[
R_H(z)=c/H(z),\qquad
\rho_\Lambda\ \text{constant},\qquad
a_T(z)=\xi G\rho_\Lambda\,c/H(z)=a_T(0)\,\frac{H_0}{H(z)}.
\]

**Correction:** with constant \(\rho_\Lambda\),
\[
\boxed{a_T(z)=a_T(0)\,\frac{H_0}{H(z)}\quad(z\le z_{\mathrm{tr}},\ \text{pause}).}
\]

That **decreases** \(a_T\) toward the past (higher \(H\)). Deep-MOND velocities at fixed baryons would be **lower** at high \(z\) than a constant-\(a_0\) law predicts.

**Alternative** if one used \(a_{(1)}\propto\sqrt{\rho}\,c\) with constant \(\rho\): \(a_T\) constant on pause — **no** high-z distinction.

**Which is forced?** Only the **shape family** \((a_{(1)},a_{(2)},a_{(3)})\). Choosing \(a_{(2)}\) gives a real seasonal rule; choosing \(a_{(1)}\) does not. Geometry of the volume constraint picks **pause** (\(\rho\) fixed) but does **not** yet pick \(G\rho R_H\) over \(\sqrt{G\rho}\,c\).

**Status of map 1:**

| Piece | Status |
|---|---|
| \(a_T\) tied to freeze density | motivated, coincidence-level |
| \(\xi\approx1.45\) | matched to locked \(a_T\), not derived |
| \(a_T(z)\propto H_0/H(z)\) on pause | **one** consistent choice (\(a_{(2)}\)) |
| Wall forces \(\xi\) | **not shown** |
| High-z RAR zero-point shift | prediction **if** \(a_{(2)}\) is adopted |

---

## 2. Σ_res from defects

### 2.1 Target

Bullet-like residual (order of magnitude):
\[
M_{\mathrm{res}}\sim 3\times10^{14}\,M_\odot
\quad\text{within}\quad
R\sim 300\,\mathrm{kpc}
\quad\Rightarrow\quad
\Sigma_{\mathrm{res}}\sim 2.5\,\mathrm{kg\,m^{-2}}
\sim 1.2\times10^9\,M_\odot\,\mathrm{kpc^{-2}}.
\]

### 2.2 Defect surface density (formula)

Degree-1 hedgehog core energy (from q0 note):
\[
E_{\mathrm{grad}}\sim C\,\mu c^2\varepsilon_\ast^2 a,
\qquad C\sim\mathcal{O}(10\text{--}50).
\]

Rest mass of one defect:
\[
m_{\mathrm{def}}=\frac{E_{\mathrm{grad}}}{c^2}\sim C\,\mu\,\varepsilon_\ast^2 a.
\]

If a projected number density of **stable** degree-1 defects is \(n_2\) (per area),
\[
\boxed{\Sigma_{\mathrm{res}}=n_2\,m_{\mathrm{def}}\sim n_2\,C\,\mu\,\varepsilon_\ast^2 a.}
\]

With Maxwell match \(\mu=\varepsilon_0\) this is electromagnetic-looking; for **gravitating** residual mass one should use the **gravitational** network stiffness, call it \(\mu_g\), not necessarily \(\varepsilon_0\).

### 2.3 Closing without a free n_2

Need \(n_2\) from geometry. Options:

1. **One defect per galaxy** in the cluster: \(n_2\sim N_{\mathrm{gal}}/(\pi R^2)\). Then \(m_{\mathrm{def}}\sim M_{\mathrm{res}}/N_{\mathrm{gal}}\). For \(N_{\mathrm{gal}}\sim 10^2\), \(m_{\mathrm{def}}\sim 10^{12}\,M_\odot\) — a **galaxy-mass** defect, not a microscopic core. That reinterprets “defect” as a **coarse-grained** cone soliton bound to each galaxy, not the lattice hedgehog of size \(a\).

2. **Microscopic lattice:** \(n_2\sim 1/a^2\) forces absurd energy unless \(\varepsilon_\ast\) is tiny. Ruled out for cluster residual.

3. **Mesoscopic:** defects densest where gradients are strongest (cluster cores, galaxies). Then \(n_2\) tracks stellar light — **same side of Bullet as CDM**. Qualitative win; quantitative \(n_2\) still not fixed.

### 2.4 Status of map 2

| Piece | Status |
|---|---|
| \(\Sigma_{\mathrm{res}}=n_2 m_{\mathrm{def}}\) | written |
| \(m_{\mathrm{def}}\sim C\mu\varepsilon_\ast^2 a\) | from existing energy matching |
| \(n_2\) fixed with no free parameter | **not achieved** |
| Qualitative: residual traces galaxies | available |
| Bullet number without free \(n_2\) | **not achieved** |

---

## 3. Combined scoreboard

| Map | Closed form written? | Coefficient derived? | New testable difference? |
|---|---|---|---|
| Roll→disk \(a_{(2)}\) | Yes | \(\xi\) matched, not derived | Yes: \(a_T(z)\propto H_0/H(z)\) on pause |
| Roll→disk \(a_{(1)}\) | Yes | O(1) | No (constant on pause) |
| \(\Sigma_{\mathrm{res}}\) | Yes as \(n_2 m_{\mathrm{def}}\) | \(n_2\) free | Qualitative only |

---

## 4. What to adopt without self-deception

**Adopt as working hypothesis (not constitution yet):**

\[
a_T(z)=a_T(0)\,\frac{H_0}{H(z)}
\quad\text{for }z\le z_{\mathrm{tr}}\sim 0.3,
\]
from map \(a_{(2)}\) + pause. This is the **first concrete seasonal rule** the spine can state. It must be stress-tested against high-z kinematics before it is locked.

**Do not lock** \(\Sigma_{\mathrm{res}}\) until \(n_2\) is fixed. Keep the formula as the definition of the residual program.

**Next calculation that would raise the floor:**
derive \(\xi\) from wall boundary condition on \(A\) or from \(\varepsilon_\ast\) normalisation in 5D — so that \(a_T\) is no longer calibrated by hand.

---

## 5. One-sentence result

We now have a **written** seasonal rule \(a_T(z)\propto 1/H(z)\) on the pause branch and a **written** residual mass formula \(\Sigma_{\mathrm{res}}=n_2 m_{\mathrm{def}}\); the first is ready to confront high-z data as a hypothesis, the second still needs a parameter-free \(n_2\).

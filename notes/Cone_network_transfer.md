# Cone-network pattern transfer

Tony Kawas / 9 September 2026. First equations. Not a photon theory yet.

Laws 1–3 stay as earlier (motion, source, conservation). Law 4: the source is deformation of the cone medium.
Boundary = allowed values of the local elongation on each cone.

This note turns the stadium-wave picture into maths. It was not already in the TAFA continuum notes.

---

## 1. Discrete network

Sites \(i\) on a lattice with spacing \(a\).

Local state: elongation \(\varepsilon_i(t)\in\mathbb{R}\) (shape change of that cone).
Allowed domain (boundary of the path):

\[
\lvert\varepsilon_i\rvert \le \varepsilon_{\max}
\]

(optional hard wall; soft version below).

Each site has a restoring potential of TAFA type, or its small-elongation quadratic floor:

\[
V(\varepsilon)=\frac12\mu\,\omega_0^2\varepsilon^2
\qquad\text{(floor of the well)},
\]

or the full wall form if needed later:
\(V(\varepsilon)=\Lambda^4\tan^2(\varepsilon/2f)\) with \(\lvert\varepsilon\rvert<\pi f\).

Neighbor coupling (energy of relative shape change):

\[
U_{\mathrm{cpl}}=\frac12\kappa\sum_{\langle i j\rangle}(\varepsilon_i-\varepsilon_j)^2.
\]

Kinetic term for the pattern (not for a particle flying through):

\[
T=\frac12\mu\sum_i \dot\varepsilon_i^2.
\]

---

## 2. Equation of motion

Euler–Lagrange:

\[
\mu\ddot\varepsilon_i
=
-\partial V/\partial\varepsilon_i
+\kappa\sum_{j\sim i}(\varepsilon_j-\varepsilon_i).
\]

With quadratic \(V\):

\[
\ddot\varepsilon_i
+
\omega_0^2\varepsilon_i
=
\frac{\kappa}{\mu}\sum_{j\sim i}(\varepsilon_j-\varepsilon_i).
\]

**Pause / active on one site**

- Active: \(\lvert\dot\varepsilon_i\rvert\) or \(\lvert\varepsilon_i\rvert\) away from equilibrium.
- Pause: local resting near \(\varepsilon_i\approx 0\) (or at a constrained waist value).

Both coexist on the network: that is the wave.

---

## 3. Continuum limit (stadium wave)

Let \(\varepsilon(\mathbf{x},t)\) with \(\mathbf{x}=a\mathbf{n}\). Nearest-neighbor Laplacian:

\[
\sum_{j\sim i}(\varepsilon_j-\varepsilon_i)\ \to\ a^2\nabla^2\varepsilon.
\]

Then

\[
\partial_t^2\varepsilon
+
\omega_0^2\varepsilon
=
\frac{\kappa a^2}{\mu}\nabla^2\varepsilon.
\]

Define

\[
c^2=\frac{\kappa a^2}{\mu}.
\]

Wave equation with a mass gap if \(\omega_0\neq 0\):

\[
\partial_t^2\varepsilon - c^2\nabla^2\varepsilon + \omega_0^2\varepsilon = 0.
\]

If the local floor is tuned so the relevant mode is effectively gapless (\(\omega_0\to 0\) for the transfer channel),

\[
\partial_t^2\varepsilon = c^2\nabla^2\varepsilon.
\]

**Lightlike speed is not inserted by hand.** It is

\[
c = a\sqrt{\kappa/\mu}
=
\frac{\text{spacing}}{\text{transfer time scale}}.
\]

That is the stadium-wave rule: nobody runs the track; the pattern’s hand-off rate sets the speed.

---

## 4. Packet as a pure process (no billiard ball)

A localized excitation

\[
\varepsilon(\mathbf{x},t)=f(\mathbf{x}-c\hat n\,t)
\]

is the “photon” in this picture: **the traveling shape**, not a site that moves.

Energy of the packet (quadratic theory):

\[
E=\int\mathrm{d}^3x\,\Bigl(\tfrac12\mu(\partial_t\varepsilon)^2+\tfrac12\mu c^2\lvert\nabla\varepsilon\rvert^2+\tfrac12\mu\omega_0^2\varepsilon^2\Bigr).
\]

Momentum density from the same stress (Law 2–3: this is the \(T_{0i}\) of the pattern).

---

## 5. Optional one-way transfer (threshold rule)

If the conceptual cycle is discrete (elongate → transfer → restore), a simple rule:

\[
\text{if }\varepsilon_i>\varepsilon_\ast\text{ and }\varepsilon_j<\varepsilon_\ast
\quad\Rightarrow\quad
\varepsilon_j\leftarrow\varepsilon_j+\delta,\quad
\varepsilon_i\leftarrow\varepsilon_i-\delta.
\]

Directionality needs an extra structure (ordered phase, spin/polarization vector, or a preferred null direction). Without that, the linear theory of §2–3 is bidirectional and closer to a real field mode.

---

## 6. Link to the single-cone volume constraint

On one cone we already had

\[
N\bigl(2 L A_\phi\,p + 1\bigr)=0
\]

(pause branch vs track branch).

On the network, a local volume label \(v_i(\varepsilon_i)\) can be constrained site by site or only in the mean. The continuum stress of §4 must still satisfy

\[
\nabla_\mu T^{\mu\nu}=0
\]

(Law 3). The wave equation above does, for the standard scalar stress tensor.

---

## 7. What this is / is not

| Claim | Status |
|---|---|
| Pattern moves; sites need not | Written |
| \(c\) from spacing and coupling | Written |
| Pause and active coexist on the lattice | Written |
| Maxwell, polarization, two-slit, \(E=h\nu\) | **Not derived** |
| Replacement for QED | **No** |

Next math step if this stays on the line: couple two polarizations (vector or complex \(\varepsilon\)), then ask whether a null packet with fixed \(E/\lvert\mathbf{p}\rvert=c\) survives the TAFA walls.

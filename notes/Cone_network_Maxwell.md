# Free Maxwell from the transverse cone network

Tony Kawas / 9 September 2026. Derivation with stated identifications.
Builds on `Cone_network_transfer.md` and `Cone_network_polarization.md`.

---

## 0. Honesty at the start

What the cone network already gave:

\[
\partial_t^2\boldsymbol{\varepsilon}-c^2\nabla^2\boldsymbol{\varepsilon}=0,
\qquad
\nabla\cdot\boldsymbol{\varepsilon}=0.
\]

That is a **transverse massless vector wave**, not yet Maxwell’s system in its usual form.

To reach free Maxwell one must **identify** \(\boldsymbol{\varepsilon}\) with a gauge potential (or with \(\mathbf{E}\)) and **define** \(\mathbf{E},\mathbf{B}\) from it. Those definitions are natural and unique up to residual gauge in Coulomb gauge; they are still identifications, not forced by the lattice spacing alone.

Sources \(\rho,\mathbf{J}\) are not produced by this note. Vacuum only.

---

## 1. Identification (Coulomb / radiation gauge)

Set units where the network speed is the light speed already written:

\[
c=a\sqrt{\kappa/\mu}.
\]

Identify the elongation with the vector potential in radiation gauge:

\[
\mathbf{A}(\mathbf{x},t)\equiv\boldsymbol{\varepsilon}(\mathbf{x},t),
\qquad
\nabla\cdot\mathbf{A}=0,
\qquad
\phi=0.
\]

(The constraint \(\nabla\cdot\boldsymbol{\varepsilon}=0\) is exactly Coulomb gauge for \(\mathbf{A}\).)

Define the electromagnetic fields by the standard kinematic map:

\[
\mathbf{B}\equiv\nabla\times\mathbf{A},
\qquad
\mathbf{E}\equiv-\partial_t\mathbf{A}.
\]\n
(With \(\phi=0\).)

---

## 2. Two homogeneous Maxwell equations (identities)

These follow from the definitions alone, with no equation of motion:

**Gauss for magnetism**

\[
\nabla\cdot\mathbf{B}
=
\nabla\cdot(\nabla\times\mathbf{A})
=0.
\]

**Faraday**

\[
\nabla\times\mathbf{E}
=
\nabla\times(-\partial_t\mathbf{A})
=
-\partial_t(\nabla\times\mathbf{A})
=
-\partial_t\mathbf{B}.
\]

So

\[
\nabla\cdot\mathbf{B}=0,
\qquad
\nabla\times\mathbf{E}=-\partial_t\mathbf{B}.
\]

---

## 3. Dynamical Maxwell equations from the wave equation

Network law (gapless transverse channel):

\[
\partial_t^2\mathbf{A}-c^2\nabla^2\mathbf{A}=0,
\qquad
\nabla\cdot\mathbf{A}=0.
\]

**Electric Gauss (vacuum)**

\[
\nabla\cdot\mathbf{E}
=
-\partial_t(\nabla\cdot\mathbf{A})
=0.
\]

**Ampère–Maxwell (vacuum)**

Use the vector identity, valid because \(\nabla\cdot\mathbf{A}=0\):

\[
\nabla\times\mathbf{B}
=
\nabla\times(\nabla\times\mathbf{A})
=
\nabla(\nabla\cdot\mathbf{A})-\nabla^2\mathbf{A}
=
-\nabla^2\mathbf{A}.
\]

From the wave equation \(\nabla^2\mathbf{A}=c^{-2}\partial_t^2\mathbf{A}\),

\[
\nabla\times\mathbf{B}
=
-\frac{1}{c^2}\partial_t^2\mathbf{A}
=
\frac{1}{c^2}\partial_t\mathbf{E}.
\]

Thus

\[
\nabla\times\mathbf{B}=\frac{1}{c^2}\partial_t\mathbf{E}.
\]

(In SI; in units \(c=1\), \(\nabla\times\mathbf{B}=\partial_t\mathbf{E}\).)

---

## 4. Free Maxwell set

Collecting:

\[
\begin{aligned}
\nabla\cdot\mathbf{E}&=0,\\
\nabla\cdot\mathbf{B}&=0,\\
\nabla\times\mathbf{E}&=-\partial_t\mathbf{B},\\
\nabla\times\mathbf{B}&=\frac{1}{c^2}\partial_t\mathbf{E}.
\end{aligned}
\]

with

\[
c=a\sqrt{\kappa/\mu}
\]

fixed by the cone-network spacing and coupling.

Polarizations of plane waves are exactly the \(\mathbf{e}^{(1)},\mathbf{e}^{(2)}\) already derived: for \(\mathbf{A}=\mathbf{e}^{(\lambda)}e^{i(\mathbf{k}\cdot\mathbf{x}-\omega t)}\) with \(\omega=c\lvert\mathbf{k}\rvert\) and \(\mathbf{e}\cdot\mathbf{k}=0\),

\[
\mathbf{B}=i\mathbf{k}\times\mathbf{A},
\qquad
\mathbf{E}=i\omega\mathbf{A},
\]

so \(\mathbf{E},\mathbf{B},\hat{\mathbf{k}}\) form a right-handed triad and \(\lvert\mathbf{E}\rvert=c\lvert\mathbf{B}\rvert\).

---

## 5. Stress and Laws 2–3

The free Maxwell stress-energy (vacuum) is the Noether stress of this quadratic theory. It satisfies

\[
\partial_\mu T^{\mu\nu}=0
\]

in the absence of charges — Law 3 for this source. Law 2 is Einstein or Newton response to that \(T^{\mu\nu}\) if gravity is coupled; this note does not couple gravity.

---

## 6. What was assumed vs obtained

| Step | Status |
|---|---|
| Transverse wave on cone network | From previous notes |
| \(\mathbf{A}\equiv\boldsymbol{\varepsilon}\), \(\phi=0\), \(\nabla\cdot\mathbf{A}=0\) | **Identification** |
| \(\mathbf{B}=\nabla\times\mathbf{A}\), \(\mathbf{E}=-\partial_t\mathbf{A}\) | **Definition** |
| \(\nabla\cdot\mathbf{B}=0\), Faraday | **Identities** from definitions |
| \(\nabla\cdot\mathbf{E}=0\), Ampère–Maxwell vacuum | **From** wave equation + Coulomb gauge |
| \(\rho,\mathbf{J}\) and full inhomogeneous Maxwell | **Not derived** |
| Uniqueness of the identification (vs \(\boldsymbol{\varepsilon}=\mathbf{E}\) directly) | Other maps exist; this one matches gauge potential + two helicities cleanly |
| Linear QED, photons as quanta | **Not derived** |

---

## 7. Compact chain

\[
\underbrace{\text{cone lattice + transverse }\boldsymbol{\varepsilon}}_{\text{network}}
\;\xrightarrow{\mathbf{A}=\boldsymbol{\varepsilon},\,\phi=0}\;
\underbrace{\square\mathbf{A}=0,\,\nabla\cdot\mathbf{A}=0}_{\text{radiation gauge}}
\;\xrightarrow{\mathbf{E}=-\partial_t\mathbf{A},\,\mathbf{B}=\nabla\times\mathbf{A}}\;
\underbrace{\text{free Maxwell}}_{\text{vacuum}}.
\]

That is the derivation of **source-free** Maxwell equations from the cone-network elongation wave, given the potential identification above.

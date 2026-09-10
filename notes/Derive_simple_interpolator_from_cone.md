# Attempt: derive simple interpolator (φ-height) from cone geometry

Tony Kawas / 10 September 2026. No SPARC input. Harden-B upgrade path.

---

## Target

Show from locked cone structure alone that the disk response must be the simple MOND form
\[
\mu(x)=\frac{x}{1+x}\qquad\Rightarrow\qquad
\left.\frac{g}{a_T}\right|_{g_N=a_T}=\varphi,
\]
without fitting galaxies.

---

## Clarification of the target form

The locked “simple interpolator”
\[
g=\tfrac12 g_N+\sqrt{(\tfrac12 g_N)^2+g_N a_T}
\]
is exactly the algebraic inverse of the standard simple
\[
\mu(x)=\frac{x}{1+x}\qquad(x=g/a_T)
\]
under the Bekenstein–Milgrom relation \(\mu(g/a_T)\,g=g_N\).
At \(g_N=a_T\) one has \(x^2-x-1=0\Rightarrow x=\varphi\).

So the derivation task is: **force \(\mu(x)=x/(1+x)\) and the constitutive law from the cone.**

---

## Routes tried

### Route 1–2 — Algebra of the formula
φ appears because of the formula. Does not derive the formula from geometry.

### Route 3 — Quadratic identity
\[
g(g-g_N)=g_N a_T
\]
is equivalent to the simple form. Suggestive bookkeeping (“observed × residual = baryonic × floor”) but not forced by an action variation.

### Route 4 — Self-similarity
φ satisfies \(y(y-1)=1\). Same algebra; no new geometric input.

### Route 5 — Volume constraint
\(N(2LA_\phi p+1)=0\) fixes cosmological branch (pause vs roll). **No map** to local disk \(\mu(g)\).

### Route 6 — Two-channel occupation (best motivation)

| Assumption | Content | Forced by locked cone? |
|---|---|---|
| A1 | Only active + pause channels | Motivated by waist ontology; not unique |
| A2 | Active occupation \(\propto g/a_T\) | **Ansatz** (could be \(x^n\)) |
| A3 | Pause occupation = const (one frozen mode/site) | Plausible from discrete freeze; not proved |
| A4 | \(\mu=\) active fraction | Natural definition |
| A5 | \(\mu(g/a_T)\,g=g_N\) | **MOND constitutive law — not derived** |

From A1–A4: \(\mu(x)=x/(1+x)\) follows.  
From A5: transition height φ follows.

**Blockers:** A2 is free; A5 is the entire MOND response law. Cone network + volume constraint + 5D warp do **not** currently imply A5.

### Route 7 — Locked numbers \(R_{\mathrm{cone}}\), \((11/72)_{\mathrm{cone}}\)
Amplitude accounting only. They do not constrain the *shape* of \(\mu(x)\).

---

## Verdict

| Claim | Result |
|---|---|
| Simple form / φ-height derived from cone action | **Fails** |
| Partial motivation (two-channel → μ form if A2+A3) | **Yes** |
| Prediction B upgraded from conditional to derivation test | **Not yet** |

**Honest status unchanged:** the simple interpolator remains a **chosen** MOND-family form. φ is exact for that choice. SPARC transition tests consistency of the choice, not a cone theorem.

---

## What would close the derivation

One of:

1. **Derive A5 from cone:** show that geodesic / stress response of the cone network yields \(\mu(g/a)\,g=g_N\) (or the quadratic \(g(g-g_N)=g_N a_T\)) from an action principle.
2. **Derive A2:** show linear occupation is forced (e.g. single-quantum pause capacity + detailed balance).
3. **Different interpolator** forced by cone that happens to have transition height φ (or another sharp, testable number).

Until one of those exists, do **not** promote B beyond conditional consistency.

---

## Do not

- Treat Route 6 motivation as a derivation.
- Reintroduce δ-dent to force SPARC median onto φ.
- Promote Prediction A as compensation.

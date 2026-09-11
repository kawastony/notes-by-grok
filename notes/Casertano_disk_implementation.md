# Casertano thin-disk integrator

Tony Kawas / 11 September 2026.

---

## Implementation

File: `artifacts/casertano_disk.py` (workspace).

**Method:** Toomre–Hankel transform = Casertano (1983) limit \(z_0 \to 0\) (razor-thin disk):

\[
S(k)=\int_0^\infty u\,\Sigma(u)\,J_0(ku)\,\mathrm{d}u,
\qquad
V_c^2(R)=2\pi G R\int_0^\infty k\,J_1(kR)\,S(k)\,\mathrm{d}k.
\]

**Units:** \(R\) in kpc, \(\Sigma\) in \(\mathrm{M}_\odot/\mathrm{pc}^2\), \(V_c\) in km/s, \(G=4.302\times10^{-6}\).

**API:**
```python
from casertano_disk import thin_disk_Vc, freeman_Vc, validate_freeman
Vc = thin_disk_Vc(R_eval, R_sig, Sigma_pc)
```

---

## Validation — Freeman (1970) exponential disk

\(\Sigma_0=100\,\mathrm{M}_\odot/\mathrm{pc}^2\), \(R_d=2\) kpc.

| \(R\) (kpc) | Analytic | Numerical | rel err |
|---|---|---|---|
| 0.5 | 17.076 | 17.023 | 0.31% |
| 1.0 | 27.185 | 27.173 | 0.05% |
| 2.0 | 38.764 | 38.769 | 0.01% |
| 3.0 | 43.963 | 43.973 | 0.02% |
| 4.0 | 45.666 | 45.677 | 0.02% |
| 6.0 | 44.054 | 44.061 | 0.02% |
| 8.0 | 40.086 | 40.083 | 0.01% |
| 10.0 | 35.974 | 35.965 | 0.03% |

**max err = 0.31%  → PASS** (criterion < 1%).

---

## Notes

- GIPSY `rotmod.c` elliptic polynomial kernel was ported but proved numerically fragile near the diagonal singularity; Hankel form is preferred for the thin limit.
- Finite-thickness Casertano (\(z_0>0\)) is not implemented; not required for SPARC-style thin-disk stellar contributions.
- Grid defaults (`kmax=100`, `nk=2000`, `nu=5000`) are tuned for Freeman PASS; denser grids may be needed for sharply truncated profiles.

---

## Next

Stage 3 audit: load `BulgeDiskDec_LTG` SB profiles, set \(\Sigma=\Upsilon\times\mathrm{SB}\) with pre-committed \(\Upsilon\), compute \(V\) with `thin_disk_Vc`, compare to Rotmod \(V_{\mathrm{disk}}\sqrt{\Upsilon}\).

# Stage 3 — dens → V rebuild vs Rotmod

Tony Kawas / 11 September 2026.

---

## Protocol

- Integrator: `casertano_disk.thin_disk_Vc` (Hankel / Casertano \(z_0\to 0\)), Freeman-validated to 0.31%.
- Dens: `BulgeDiskDec_LTG.zip` — `SBdisk` [\(\mathrm{L}_\odot/\mathrm{pc}^2\)], radii [kpc].
- Compare at **Υ = 1** to Rotmod `Vdisk` (SPARC convention: Rotmod stellar columns are Υ=1).
- Metric: median \(|V_{\mathrm{rec}}-V_{\mathrm{rot}}|/V_{\mathrm{rot}}\) over radii with \(V_{\mathrm{rot}}>5\) km/s.

---

## Result (175 galaxies)

| Quantity | Value |
|---|---|
| Median of per-galaxy med-rel-err | **58%** |
| Mean | 77% |
| Fraction < 10% | 4% |
| Fraction < 20% | 15% |
| Fraction < 50% | 43% |
| Median \(V_{\mathrm{rec}}/V_{\mathrm{rot}}\) | **1.51** (systematic high) |

**Best matches** (few %): F583-4, UGC05999, UGC04305, DDO154, PGC51017 — mostly low-SB / dwarf disks.

**Worst** (>>100%): high-SB massive spirals (NGC5907, NGC4217, …).

---

## Interpretation

| Claim | Status |
|---|---|
| Freeman validation of integrator | Still **PASS** |
| Independent pipeline reproduces Rotmod to a few % | **FAIL** (median 58%) |
| Ready for external MAE with this rebuild | **Not yet** |

Likely contributors (not yet isolated):

1. **Finite thickness** — SPARC/Casertano with \(z_0>0\) lowers \(V\) vs razor-thin; our code is thin-only.
2. **Sampling / taper** — Hankel grid defaults may under-resolve compact high-SB centres.
3. **Unit / zero-point** of dens \(\mathrm{L}_\odot/\mathrm{pc}^2\) vs the mass model SPARC used for Rotmod (less likely given header, but not ruled out).

---

## Discipline

This is reported as a **failed few-percent consistency check**, not dropped. The tool remains valid for the exponential benchmark; it is **not** yet a drop-in replacement for Rotmod on the full SPARC sample.

**Next options:**

1. Add finite-thickness Casertano (\(z_0 \sim 0.2 R_d\)) and re-compare.
2. Restrict rebuild trust to low-SB dwarfs where agreement is already good; use Rotmod elsewhere.
3. External test only with published professional decompositions (when available), not home rebuild.

Until (1) or published external \(V_{\mathrm{bar}}\), Stage 4 remains blocked for a fair MAE.

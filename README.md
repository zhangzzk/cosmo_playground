# Cosmo PlayGround: pyccl Notebook Suite

Minimal notebook-only project for cosmology parameter-response studies.

## Active Notebooks

- `notebooks/00_basic_cosmology.ipynb`
- `notebooks/01_shear_cl_component.ipynb`
- `notebooks/02_gammat_cl_component.ipynb`
- `notebooks/03_gg_cl_component.ipynb`

## Scientific Scope

- Basic cosmology notebook shows: comoving distance, growth, transfer-shape proxy from linear power, linear/nonlinear matter power, and HMF (if available in local `pyccl` build).
- 3x2pt component notebooks show harmonic-space responses for:
  - shear: `C_ell^{gamma gamma}`
  - galaxy-shear: `C_ell^{g gamma}`
  - galaxy clustering: `C_ell^{g g}`

## Notes on Correctness

- `T_proxy(k)` is a transfer-shape proxy derived from `P_lin(k)`; it is not the raw Boltzmann transfer output.
- Default transfer model is set to `eisenstein_hu` for robustness (no external CLASS requirement).
- Tomography uses pedagogical Smail `n(z)` + top-hat binning + optional per-bin photo-z shifts.

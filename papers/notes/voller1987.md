# Reading note — Voller & Prakash (1987), R16

**Paper:** V. R. Voller and C. Prakash, *A fixed grid numerical modelling
methodology for convection-diffusion mushy region phase-change problems*,
International Journal of Heat and Mass Transfer 30(8), 1709–1719, DOI
`10.1016/0017-9310(87)90317-6`.

## Claim

A fixed-grid enthalpy formulation can represent a mushy phase-change region by
treating the two-phase zone as a porous medium with a Darcy-type momentum
source that vanishes in the fully liquid phase.

## What this portfolio takes

- The **enthalpy–porosity method** is the benchmark for the self-written solver
  in E03 (W09–W13) and its 2D extension in E07 (W27–W35).
- The mushy-zone source term is the mechanism that makes the solver a physics
  solver rather than a generic PDE demo.
- Benchmark cases from the paper will be reproduced before any alloy-specific
  case is attempted.

## Numbers / statements to reproduce

| Quantity | Target | Where it will be reported |
|---|---|---|
| Front position vs analytical solution | error < 2% | W11, `benchmarks/stefan.csv` |
| Energy conservation | < 0.5% | W12, V&V report |
| Benchmark reproduction | qualitative + quantitative match | W30, `benchmarks/voller_prakash.md` |

## Limitations of this note

Equations and numerical parameters have **not** yet been transcribed from the
paper. Do not implement the source term from this note alone; read the original
notation and record it here before W09.

**Status:** to be completed before W09.

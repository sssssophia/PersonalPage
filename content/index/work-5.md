---
number: 05
title: Calibration & Response Optimisation
tags: Calibration Loops | Correlation Analysis | Simulation Comparison | System Optimisation
methods: correlation tracking, rotation-based correction, response calibration
impact: used interpretable correlations to reduce response bias and stabilise calibrated outputs.
industry: Calibration Systems | Digital Twins | Engineering Optimisation
evidence_title: Selected evidence from project work
---
Reduced response bias by turning a persistent correlation into an explicit calibration signal.

- Measured how the response parameter `a` varies with energy instead of assuming a constant response model.
- Used that structure to define a simple rotation-based correction for the normalised response.
- Kept the correction interpretable so behaviour could be validated across detector configurations and operating points.

## Evidence
- The `E_vs_a.pdf` slides isolate the `Energy vs a` correlation as a named calibration problem, then follow it with a dedicated `Rotation` correction step.
- The stated correction uses a rotation point at `f_em = 1.0` and a simple transformed response of the form `n_norm + (1 - f_em) * a`, making the optimisation logic explicit.

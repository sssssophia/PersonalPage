---
number: 02
title: Time-Series Inference
tags: Time-Series Modelling | Bias Correction | Calibration | Joint Fitting
methods: decay-time acceptance modelling, resolution calibration, simultaneous fitting
impact: improved time-dependent inference by separating acceptance, resolution, and calibration effects across datasets.
industry: Retention Analytics | Churn Modelling | Causal Inference
evidence_title: Selected evidence from project work
---
Built a time-series inference workflow for data affected by selection effects, detector resolution, and sample mismatch.

- Modelled acceptance and resolution explicitly instead of absorbing reconstruction effects into a single nuisance term.
- Estimated Run 1 and Run 2 corrections separately to avoid over-sharing assumptions across datasets.
- Calibrated the effective time resolution with control samples and propagated residual mismodelling as systematic uncertainty.

## Evidence
- The note states that signal and control samples were matched by GB reweighting before building the acceptance correction, rather than assuming raw MC agreement.
- Acceptance extraction combined `B0` data, `B0/Bs0` MC ratios, and a simultaneous fit; Run 1 and Run 2 were treated separately to avoid over-sharing detector response assumptions.

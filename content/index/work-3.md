---
number: 03
title: Domain Adaptation for ML
tags: GBDT | XGBoost | Reweighting | Feature Validation
methods: BDT validation, gradient-boosting reweighting, calibration-sample alignment
impact: reduced kinematic mismatch between calibration and signal-like samples before downstream modelling and selection.
industry: Domain Adaptation | Production ML | Dataset Shift
evidence_title: Selected evidence from project work
---
Improved model robustness under distribution shift by validating score behaviour and reweighting samples before downstream use.

- Used train-test BDT score comparisons to check separation quality and overtraining behaviour.
- Reweighted calibration and control samples so their kinematics better matched the target signal sample.
- Treated reweighting as part of the validation loop whenever downstream inference depended on sample agreement.

## Evidence
- The `Run2_Bs2PhiGamma_TestTrain.pdf` plot explicitly compares signal/background train and test BDT responses, providing a direct diagnostic of model behaviour before threshold optimisation.
- In the time-dependent note, calibration decays in both data and simulation were reweighted with a GBR so observables such as `pT(B)` and `eta(B)` matched the signal channel more closely.

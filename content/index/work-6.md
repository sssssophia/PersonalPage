---
number: 06
title: Data Quality Monitoring
tags: Monitoring | Data Validation | Performance Diagnostics | Root-Cause Analysis
methods: benchmark-channel checks, MC-data comparison, detector-level diagnostics
impact: identified reconstruction anomalies and translated them into concrete calibration, alignment, and software follow-ups.
industry: Production Monitoring | Model Validation | Observability | Quality Assurance
evidence_title: Selected evidence from project work
---
Built a production-style validation workflow for early Run 3 photon reconstruction, focused on finding actionable detector and software issues.

- Used multiple high- and low-momentum photon channels as benchmark datasets for reconstruction and identification checks.
- Compared MC and data across trigger streams and offline selections to isolate where discrepancies entered the pipeline.
- Traced anomalies back to concrete causes, including problematic ECAL cells, imperfect alignment/calibration, and a missing-HCAL-energy bug later fixed in software.

## Evidence
- The Run 3 performance note explicitly uses `Bs -> phi gamma`, `Bd -> K* gamma`, and charmonium channels as benchmark datasets for validating photon and `pi0` performance in early data.
- The study documents concrete findings rather than generic monitoring: an abnormal bump linked to a specific ECAL cell, asymmetries in inner-ECAL photon distributions, and a missing-HCAL-energy issue fixed in `Rec v35r18`.

---
number: 07
title: Simulation Correction Tooling
tags: Scientific Software | Event Filtering | Simulation Correction | Framework Integration
methods: Gaudi-package development, event-level correction, framework integration
impact: turned theory-driven correction factors into a reusable software package for improving simulation realism.
industry: Simulation Platforms | Scientific Computing | Data Engineering
evidence_title: Selected evidence from project work
---
Developed simulation-correction tooling that turns measured physics constraints into an event-level resampling workflow.

- Built a Gaudi-based package under the BOSS framework to correct inclusive `D0 Dbar0` simulation samples event by event.
- Encoded correction factors from measured inputs into a filtering workflow that keeps or rejects events to match the corrected distribution.
- Designed the package so the correction logic is reusable beyond a single analysis or software stack.

## Evidence
- The QCFilter report describes `QCMCFilterAlg` as a new Gaudi-based package developed to improve `D0 Dbar0` simulation at BESIII through quantum-coherent correction.
- The event-level logic is explicit: each event receives a correction factor and is kept or discarded by comparing that value to a random number, making the software behaviour auditable and portable.

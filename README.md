# TLC-Calib: Robust Multi-View Extrinsic Calibration with Limited Co-observations

This repository provides the reference implementation of **TLC-Calib**, a sparse graph reprojection-based framework for **extrinsic calibration of fixed multi-camera systems under limited co-observations**, including **non-overlapping/weak-overlap FoV** and **missing/insufficient loop-closure** conditions.

It accompanies the IEEE TIM paper:

> **Robust Multi-View Extrinsic Calibration with Limited Co-observations via Sparse Graph Reprojection and Target-Driven Loop Closure**  
> <Guanhua Chen, Fengdong Chen, Guodong Liu, Yueyue Han and Kejun Li>, IEEE Transactions on Instrumentation and Measurement, <2026>.  
> (Early Access / DOI: <to be added>)

---

## Key Features

- **Fixed multi-camera extrinsic calibration** under sparse simultaneous co-observations
- **Sparse graph reprojection** with a unified modeling of simultaneous co-observation constraints
- **Target-driven loop closure** to mitigate drift in chain-like / weak-loop topologies
- Compatible with **composite multi-plane target groups** (rigidly connected planar targets)
- Evaluation on **simulation** and **real-world platforms** (as reported in the paper)

---

## Repository Status

- ✅ Codebase: **in preparation for public release**
- ✅ Paper link / citation: **available**
- ⏳ Example datasets and full scripts: **to be released**
- ⏳ One-click reproduction: **to be released**

> We are actively cleaning the code and organizing datasets/scripts to ensure reproducibility.  
> The final release will include documented pipelines and example data consistent with the paper.

---

## Method Overview (High-Level)

TLC-Calib follows a two-stage pipeline:

1. **Local estimation:** compute relative transformations from limited simultaneous co-observations.
2. **Global optimization:** refine all camera extrinsics via sparse graph reprojection, while introducing target-driven loop-closure edges to improve observability and suppress drift.

For details, please refer to the paper.

---

## Getting Started

### Requirements
- Python: `== 3.11`
  - g2o-python: `>=0.0.12`
  - aprilgrid: `>=0.3.0`
  - open3d: `>=0.18.0`

> **Note:** The exact dependency list will be provided in the first public release.

### Installation (Placeholder)
```bash
git clone https://github.com/Regentropfen-hit/TLC-Calib.git
cd TLC-Calib
# TODO: installation steps will be added

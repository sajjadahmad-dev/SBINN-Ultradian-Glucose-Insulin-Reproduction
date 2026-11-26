
SBINN ULTRADIAN GLUCOSE-INSULIN EXPERIMENT
=========================================

Implementation:
Updated Lu Group SBINN PyTorch implementation.

Original assigned reference:
Yazdani et al. (2020),
Systems biology informed deep learning
for inferring parameters and hidden dynamics.

Training:
1000 supervised steps
3000 physics-informed steps
4000 total optimization steps

Forward glucose trajectory reconstruction:
RMSE: 0.751931
MAE: 0.353544
Relative L2: 0.006690

Inverse parameter estimation:
17 parameters in comparison
14 changed during optimization
3 unchanged: a1, C1, C2

MAPE across all 17: 23.322%
MAPE across 14 changed: 28.320%

IMPORTANT LIMITATIONS:
- Results are based on the updated SBINN implementation.
- This is not an exact reproduction of all 2020 experiments.
- Glucose error is measured on the training time interval.
- Independent future forecasting has not been validated.
- Unchanged parameters were initialized at reference values.
- A good trajectory fit does not establish parameter recovery.
- Results should be reported as preliminary reproduction.

FOLDER CONTENTS:
figures/         Generated experimental plots
tables/          Metrics and parameter comparisons
source_code/     Experiment source files
experiment_data/ Numerical data and training outputs

Source:
https://github.com/lu-group/sbinn

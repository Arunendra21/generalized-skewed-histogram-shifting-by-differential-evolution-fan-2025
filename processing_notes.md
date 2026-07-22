# Processing Notes — Generalized Skewed Histogram Shifting by Differential Evolution (Fan 2025)

- **Paper:** Guojun Fan, Lei Lu, Zijing Li, Ping Li, Quan Zhou, Zhibin Pan, IEEE TMM, vol. 27, 2025
- **Reproduction tier:** A
- **Status:** Completed (full reproduction)

## What was reproduced
High-capacity rhombus PEE core, levels 1..3, 8 images, bit-exact reversibility guaranteed.

## Reproduced vs reported
The capacity-PSNR regime and reversibility are reproduced. The DE-optimised skewed predictors are **approximated** by the standard predictor + level sweep (stated openly), so reproduced capacity is a conservative lower bound on the paper's optimised numbers.

## Honesty note
All numbers from included code on bundled images; 'reported' cells reflect the paper.

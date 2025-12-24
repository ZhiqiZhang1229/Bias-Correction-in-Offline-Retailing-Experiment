# Bias Correction in Offline Retailing Experiments: Theory and Empirical Evidence
This repository open-sources the code and data needed to reproduce the empirical and simulation results in **“Bias Correction in Offline Retailing Experiments: Theory and Empirical Evidence”**.

## Table of Contents
- [Overview](#overview)
- [Reproducing Results](#reproducing-results)
- [Data](#data)
- [Data Dictionary](#data-dictionary)

## Overview
The empirical materials in this repository include the code and datasets required to generate all reported figures, tables, and numerical results in the paper.

## Reproducing Results
The following notebooks reproduce the corresponding tables in the paper:

- **Table 2: Error of GTE Estimators across DGPs**  
  `LinearMNL.ipynb`, `NestedLinearMNL.ipynb`, `MixedLogit.ipynb`, `Nonparametric.ipynb`, `Complementarity.ipynb`

- **Table 3: Sensitivity Analysis — Comparative Performance (MAPE %) under Mixed Logit DGP**  
  `LinearMNL.ipynb`, `NestedLinearMNL.ipynb`, `MixedLogit.ipynb`, `Nonparametric.ipynb`, `Complementarity.ipynb`, `Numeric Study.ipynb`

- **Table 4: Variable Definitions and Randomization Checks** (and power analysis results)  
  `Data_and_Power.ipynb` with `no_discount.csv`, `all_discount.csv`, `half_discount.csv`

- **Table 5: Average Treatment Effect of Price Discounts**  
  `Empirical_Evidence.ipynb` with `no_discount.csv`, `all_discount.csv`

- **Table 6: Bootstrap Comparison Across Methods**  
  **and** **Table 7: Percentage of 95% CIs Covering the Ground-Truth GTE**  
  `GTE_Evaluation.ipynb` with `no_discount.csv`, `all_discount.csv`, `half_discount.csv`, `product.csv`

## Data
This repository includes the following datasets:
- `no_discount.csv`
- `all_discount.csv`
- `half_discount.csv`
- `product.csv`

## Data Dictionary
- `no_discount.csv`: Consumer features and purchase choices for participants in the **No Discount** condition.
- `all_discount.csv`: Consumer features and purchase choices for participants in the **All Discount** condition.
- `half_discount.csv`: Consumer features and purchase choices for participants in the **Half Discount** condition.
- `product.csv`: Product-level features, prices, and treatment assignment.

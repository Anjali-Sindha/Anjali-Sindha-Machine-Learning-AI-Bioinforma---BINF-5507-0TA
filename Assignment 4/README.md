# README: Survival Analysis Pipeline with Python

## Overview

This project implements a **survival analysis pipeline** for clinical data using Python. The workflow covers data loading, cleaning, Kaplan-Meier analysis, Cox proportional hazards regression, and Random Survival Forests (RSF), with automated plotting and reporting. The code is modular, well-commented, and outputs all results to a dedicated `plots` directory for easy review.

## Features

- **Data Preparation**: Cleans and encodes clinical data, prepares survival time and event indicators.
- **Kaplan-Meier Analysis**: Plots survival curves by treatment modality and tumor stage, with log-rank test results for group comparisons.
- **Cox Proportional Hazards Model**: Fits a Cox model (stratified by stage), checks proportional hazards assumptions, and saves a detailed summary.
- **Random Survival Forest (RSF)**: Trains an RSF model, computes permutation-based variable importance, and compares model performance (C-index) to Cox regression.
- **Automated Output**: All plots and statistics are saved in the `plots` folder.


## How to Run

1. **Place your clinical data CSV** at the path specified by `file_path` in the script.
2. **Run the script**. It will:
   - Load and clean the data.
   - Generate and save Kaplan-Meier survival plots.
   - Fit and summarize a Cox proportional hazards model.
   - Check and save proportional hazards assumptions.
   - Train and evaluate a Random Survival Forest, saving variable importance and C-index comparisons.
   - Save all outputs (plots, tables, and summaries) in the `plots` directory.

## Output Files

- **Survival Curves**:
  - `plots/km_tx_modality.png` — Kaplan-Meier by treatment modality
  - `plots/km_stage.png` — Kaplan-Meier by tumor stage
- **Cox Model**:
  - `plots/cox_summary.txt` — Model summary
  - `plots/cox_ph_assumption.txt` — Proportional hazards assumption check
- **Random Survival Forest**:
  - `plots/rsf_variable_importance.csv` — Variable importance (permutation)
  - `plots/rsf_variable_importance.png` — Bar plot of variable importance
- **Model Comparison**:
  - `plots/cindex_comparison.txt` — C-index for RSF and Cox models

## Main Script Structure

- **Data Loading & Cleaning**: Handles missing values, encodes categorical variables, prepares time/event columns.
- **Kaplan-Meier Analysis**: Plots and log-rank tests for group comparisons.
- **Cox Regression**: Model fitting, summary, and assumption checks.
- **Random Survival Forest**: Model training, permutation importance, and performance evaluation.
- **Visualization & Saving**: All results saved to `plots` for reproducibility.

## Notes

- All statistics and tables are printed to the console and saved as files.
- The code is modular for easy extension or adaptation to new datasets.

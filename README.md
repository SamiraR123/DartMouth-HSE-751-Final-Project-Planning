# Week 3: Dataset Selection and Final Project Planning Lab
## Overview
This repository contains the dataset selection, exploratory analysis, and project planning for my HSE 751 final course project. The goal of this lab was to identify a dataset suitable for binary classification, explore its structure and quality, and plan the prediction problem I'll build on later in the course.

## Dataset
**Name:** CDC Diabetes Health Indicators
**Source:** UCI Machine Learning Repository, [https://archive.ics.uci.edu/dataset/891](https://archive.ics.uci.edu/dataset/891/cdc+diabetes+health+indicators)
**Size:** 253,680 respondents, 21 predictor variables, 1 binary target (`Diabetes_binary`)

The dataset is drawn from the CDC's 2015 Behavioral Risk Factor Surveillance System (BRFSS) survey and includes demographic, socioeconomic, behavioral, and self-reported health-status variables.


## How to Run
1. Open `Week3_final_project_planning_lab_SR.ipynb` in Google Colab (or Jupyter).
2. Run all cells in order, top to bottom. The first code cell installs the `ucimlrepo` package and pulls the dataset directly from UCI, no manual download needed.
3. All descriptive statistics, visualizations, and data quality checks regenerate from that single data pull.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VtBSkCA6JbquPR17_CixICc4XeANtTAy?usp=sharing)

## Notebook Contents
1. **Data Selection**: dataset name, source, and justification for selection
2. **Dataset Exploration**: import, structure, target variable identification, predictor descriptions, descriptive statistics, and two exploratory visualizations
3. **Data Quality Assessment**: missing value check, out-of-range/improperly coded value check, anticipated preprocessing steps, and potential challenges
4. **Project Planning**: proposed prediction problem, target variable, and candidate evaluation metric

## Key Findings
- No missing values and no improperly coded observations were found in any column.
- The target variable is imbalanced (~86% no diabetes, ~14% diabetes/prediabetes), which informs the choice of recall and AUC-ROC over raw accuracy as evaluation metrics going forward.
- Diabetes/prediabetes prevalence declines fairly steadily as income category rises within this sample.

## GenAI Disclosure
AI assistance (Claude) was used to help with the python code, strengthen the writeups, and organize this README. All data decisions, code execution, and final analysis are my own.

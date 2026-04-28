# Data Analysis

This folder contains notebooks for analyzing response times and call characteristics before and after the August 2024 MCSLC rollout.

## Purpose

The goal of this stage is to:
- Compare response times before and after the MCSLC rollout
- Analyze changes across response stages
- Examine changes in dispatch reason and disposition
- Compare response patterns where CAHOOTS and EPD data are available
- Create visualizations and statistical summaries for the final project

## Folder Contents

- `response_time_analysis.ipynb`: Compares request to dispatch, dispatch to arrival, and arrival to engagement times before and after the rollout.
- `call_type_analysis.ipynb`: Analyzes changes in dispatch reason, disposition, city, and agency response patterns.
- `statistical_tests.ipynb`: Runs t-tests for response time differences and chi-square tests for categorical differences.

## Input Files

N/A

## Output Files

N/A

## How to Run

Run the Jupyter notebooks in the following order:

1. `response_time_analysis.ipynb`
2. `call_type_analysis.ipynb`
3. `statistical_tests.ipynb`

## Dependencies

This project uses the following Python packages:

- pandas
- numpy
- matplotlib
- seaborn
- scipy

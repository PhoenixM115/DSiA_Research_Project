# Data Cleaning

This folder contains notebooks for cleaning and preparing the raw CAD, CAHOOTS, EPD, and MCSLC response data for analysis.

## Purpose

The goal of this stage is to:
- Clean and standardize raw emergency response call data
- Select the variables needed for response time and call type analysis
- Convert timestamp columns into usable datetime formats
- Align labels across datasets when possible
- Create a before/after rollout variable for the August 2024 MCSLC rollout
- Output structured CSV files for analysis

## Folder Contents

- `data_cleaning.ipynb`: Loads raw CAD and MCSLC data, fixes formatting issues, standardizes columns, handles missing values and outliers, and outputs a cleaned dataset.
- `label_alignment.ipynb`: Aligns dispatch reason, disposition, city, and agency labels across datasets where possible.
- `response_time_processing.ipynb`: Recalculates or verifies response time intervals such as request to dispatch, dispatch to arrival, and arrival to engagement.

## Input Files

- Raw CAD data files
- Raw MCSLC dispatch and response data
- CAHOOTS and EPD data, if available

## Output Files

- `cleaned_response_data.csv`: Cleaned and merged response dataset
- `cleaned_mclsc_data.csv`: Cleaned MCSLC-only dataset
- `aligned_call_labels.csv`: Dataset with standardized dispatch reason and disposition labels

## How to Run

Run the Jupyter notebooks in the following order:

1. `data_cleaning.ipynb`
2. `label_alignment.ipynb`
3. `response_time_processing.ipynb`

## Dependencies

This project uses the following Python packages:

- pandas
- numpy
- matplotlib
- seaborn
- scipy

Standard library modules used:

- datetime
- re

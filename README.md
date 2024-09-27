# README: Aircraft Accident Analysis for Risk-Based Recommendations (1963-2023)

## Project Overview

This project aims to analyze aircraft accident data from 1963 to 2023 to assist a company in determining the **lowest-risk aircraft** for purchase and operation. By leveraging a dataset of aircraft accidents, the goal is to identify trends in accident frequencies and severities across different aircraft types, providing data-driven insights for decision-making.

The analysis includes statistical tests, data visualizations, and detailed recommendations to help guide the company's selection process for the safest aircraft based on historical accident data.



## Project Structure

- **data/**: Folder containing the dataset used for analysis (`AviationData.csv`).
- **scripts/**: Python scripts for data preprocessing, analysis, and visualization.
  - `import pandas as pd`
`: Handles data cleaning and preparation.
  - ` numpy as np`
`: Contains the code for statistical tests, summary statistics, and key computations.
  - ` matplotlib.pyplot`: Generates visualizations to provide insights into the data.
- **README.md**: This file, providing an overview of the project.
- **requirements.txt**: Lists the Python packages required to run the project.

---

## Dataset Overview

The dataset consists of historical aircraft accident data from 1963 to 2023, including fields such as:
- **Make**: Manufacturer of the aircraft.
- **Model**: Model of the aircraft.
- **Aircraft Type**: Combined field of `Make` and `Model`.
- **Accident Date**: Date of the accident.
- **Severity**: Severity of the accident (e.g., "No Fatalities," "Low," "Medium," "High").
- **Location**: Where the accident occurred.
- **Injuries/Fatalities**: Number of people injured or killed.

---

## Methodology

The project follows these steps to achieve its objectives:

1. **Data Preprocessing**:
   - Clean and preprocess the dataset to handle missing values, inconsistencies, and outliers.
   - Combine the `Make` and `Model` columns to create the `Aircraft_type` column.
   - Filter relevant columns and focus on aircraft types with substantial data points.

2. **Fatality Rate Metrics**
    -Number of fatalities per accident for each aircraft type.
    - Incident Severity : Classify accidents by severity (minor, major, fatal).

3. **Accident Rate Analysis**:
   - Calculate accident rates for each aircraft type to determine which models have the highest and lowest accident frequencies.with respective graphs

4. **Ranking Scores For Aircrafts**:
 -Here we  rank Aircraft by accident rate ,Fatility rate and Severity Scores

5. **Statistical Analysis**:
   - Identify the 10 aircraft types with the highest number of accidents and calculate their severity distribution.

6. **Conclusion**:
   - Graphs: Visualize accident rates, severity, and causes for each aircraft type.

---

## Business Recommendations

Based on the analysis, the following recommendations are made to the company for selecting the lowest-risk aircraft:

- Prioritize aircraft types with high percentages of **"No Fatalities"** and **low accident counts**.
- Aircraft models such as ***Boeing*** and ***Grumman*** have a high rate of minor accidents but generally low severity, making them potentially safer choices.
- Avoid aircraft models with a higher proportion of severe or fatal accidents.

---


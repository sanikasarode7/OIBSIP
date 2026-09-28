# Unemployment Analysis with Python

## Overview

This project analyzes unemployment trends in India using exploratory data analysis and data visualization. The analysis focuses on regional differences, monthly unemployment trends, and changes between the pre-COVID and COVID-19 periods.

## Objective

To explore unemployment patterns across regions and over time, with a focus on understanding changes during the COVID-19 period.

## Dataset

The dataset contains unemployment-related information for different regions of India.

### Main Features

- Region
- Date
- Frequency
- Estimated Unemployment Rate (%)
- Estimated Employed
- Estimated Labour Participation Rate (%)
- Area

The dataset covers the period from May 2019 to June 2020 and contains both rural and urban observations.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Data Preparation

The dataset was inspected for its shape, data types, missing values, and duplicate records.

The following preprocessing steps were performed:

- Removed completely blank rows.
- Cleaned extra spaces from column names.
- Converted the Date column to datetime format.
- Checked for missing values.
- Checked for duplicate records.

After removing blank rows, the dataset contained 740 records.

## Exploratory Data Analysis

### 1. Region-wise Average Unemployment

The average unemployment rate was calculated for each region to compare regional unemployment levels.

### 2. Month-wise Unemployment Trends

Monthly average unemployment rates were calculated to examine changes in unemployment over time.

### 3. Unemployment Trends Across Selected Regions

A time-series line chart was created to compare unemployment rates over time for:

- Maharashtra
- Karnataka
- Tamil Nadu

### 4. Top 10 Regions by Average Unemployment

A bar chart was created to identify the ten regions with the highest average unemployment rates during the period covered by the dataset.

### 5. Correlation Analysis

A correlation heatmap was created to examine the relationships between:

- Estimated Unemployment Rate
- Derived Estimated Employment Rate
- Estimated Labour Participation Rate

The employment rate used in this analysis was derived from the available unemployment and labour participation rate values.

### 6. Pre-COVID vs. Post-COVID Comparison

The data was divided into two periods:

- Pre-COVID: Before March 2020
- Post-COVID: March 2020 onward

The average unemployment rate was then calculated for both periods.

The analysis shows an average unemployment rate of approximately:

| Period | Average Unemployment Rate |
|---|---:|
| Pre-COVID | 9.51% |
| Post-COVID | 17.77% |

## Key Observations

- Unemployment rates vary considerably across regions.
- Monthly unemployment rates change throughout the period covered by the dataset.
- The selected regions show different unemployment patterns over time.
- The top 10 regions have comparatively higher average unemployment rates.
- The correlation analysis shows relationships between unemployment, derived employment, and labour participation.
- The average unemployment rate was higher in the post-COVID period than in the pre-COVID period.

## Project Structure

```text
Task_2_Unemployment_Analysis/
├── Unemployment_Analysis.ipynb
├── Unemployment in India.csv
└── README.md

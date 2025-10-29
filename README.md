# Data-Science-Programming
Python-based data preprocessing project converting raw customer CSV data into structured JSON files. Includes data cleaning, nested structuring, and derived metrics like salary-per-commute. Features anomaly detection and Seaborn visualisations for analysing trends in age, salary, and employment.


The project simulates a real-world business scenario where a company needs to prepare large volumes of customer information for further analysis. The data, originally stored in a flat CSV file (acw_user_data.csv), contains various attributes such as customer demographics, financial details, vehicle information, and employment status. However, this raw dataset is not suitable for direct analytical use, as it lacks structure, consistency, and derived metrics.

To address these issues, a robust Python-based data processing pipeline was implemented using standard libraries (csv, json, os, sys, etc.). The pipeline performs a sequence of essential preprocessing tasks, including:

  1. Reading and cleaning data to handle missing or invalid entries (e.g., dependants column errors).

  2. Structuring flat data into nested representations such as Vehicle, Credit Card, and Address objects.

  3. Segregating data into multiple JSON outputs (processed.json, retired.json, employed.json, remove_ccard.json, and commute.json) for specific analytical needs.

  4. Deriving new metrics such as the Salary-Commute ratio, enabling performance ranking of customers based on income relative to travel distance.

  5. Identifying anomalies, such as credit card records with unrealistic validity periods (greater than 10 years).

In addition, the second phase of the project introduces data visualisation using Pandas and Seaborn, allowing insights into customer demographics and trends. Statistical measures (e.g., mean salary, median age) are calculated, and both univariate and multivariate plots are generated to explore relationships between variables such as age, salary, commute distance, and marital status.

Through this project, the complete data pre-processing lifecycle — from data ingestion and transformation to feature derivation and visual analysis — is demonstrated. It highlights the importance of clean, structured, and well-documented data preparation as a foundational step for subsequent machine learning and AI-based modelling.

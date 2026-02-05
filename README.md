# 🚗 Exploratory Data Analysis (EDA) of Automotive Pricing

## 🎯 Project Overview

This project focuses on conducting an Exploratory Data Analysis (EDA) on a comprehensive dataset of cars to understand the distribution of key features (such as fuel economy, horsepower) and to determine the primary relationships that influence the **Manufacturer's Suggested Retail Price (MSRP)** of vehicles.

The goal is to transform raw vehicle data into actionable business intelligence by identifying the most significant economic drivers of car value.

## 💾 Dataset

The analysis utilizes a dataset containing automotive specifications and pricing. Key columns relevant to the analysis include:
* `Engine HP`: Engine Horsepower
* `Engine Cylinders`: Number of cylinders
* `City MPG`, `Highway MPG`: Fuel consumption metrics
* `MSRP`: Manufacturer's Suggested Retail Price (The Target Variable)

Before you run notebook, please download the dataset and insert it into the notebook: 
[Car Dataset](https://drive.google.com/file/d/19V7VjHs4J8idTko7NQUT95ZJO2ZQSGWh/view)

## 🛠️ Methodology and Steps

1.  **Data Cleaning & Preprocessing:**
    * Handling of missing values (e.g., imputation for `Market Category`, removal of rows with missing critical numeric data).
    * Standardization of column names.
    * **Outlier Removal:** Outliers in the target variable (`MSRP`) were addressed to ensure robust statistical analysis.
2.  **Feature Engineering:**
    * Creation of new, more informative features, such as `total_mpg` (aggregated fuel efficiency) and `price_per_HP` (normalized price metric).
3.  **Exploratory Data Analysis (EDA):**
    * Statistical summaries and distribution plots.
    * **Correlation Analysis (Heatmap):** Used to quantify the relationships between all variables.
    * Visualizations (scatter plots, line plots) to examine key dependencies, particularly between `Engine HP` and `MSRP`.

## 💡 Key Findings

The analysis yielded the following critical insights:

* **Primary Price Driver:** **Engine Horsepower (Engine HP)** exhibits the strongest positive correlation with MSRP (Coefficient: **0.65**). This conclusively identifies Engine HP as the most influential factor in determining the vehicle's retail price.
* **Performance vs. Efficiency:** A moderate negative correlation (approx. -0.45) was observed between Engine HP and fuel efficiency (MPG), confirming the typical trade-off between power and fuel economy.
* **Fuel Efficiency:** A very strong positive correlation (0.89) exists between City MPG and Highway MPG.

## 🚀 Conclusion

This project successfully established a clean, analyzed dataset and clearly identified **Engine HP** as the dominant economic driver of vehicle pricing. The comprehensive EDA serves as an essential foundation for the next phase, which would involve developing a predictive machine learning model (e.g., a Regression Model) for accurate MSRP forecasting.

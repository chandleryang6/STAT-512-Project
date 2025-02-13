# STAT-512-Project: U.S. Renewable Energy Consumption Analysis 
A Multiple Linear Regression study using US and global renewable energy datasets. This project analyzes the impact of different renewable energy sources on total renewable energy consumption in the U.S. from 1980 to 2021. The primary goal is to determine whether the combined influence of solar, wind, biomass, and hydroelectric power explains the growth in renewable energy consumption. 

## Datasets and Variables
The dataset used is: 
- [U.S. Renewable Energy Consumption](https://www.kaggle.com/datasets/alistairking/renewable-energy-consumption-in-the-u-s)
- **Timeframe**: 1980-2021
- **Key Variables**:
  - **Y (Target Variable):** Total Renewable Energy
  - **X₁:** Solar Energy
  - **X₂:** Wind Energy
  - **X₃:** Biomass Energy
  - **X₄:** Hydroelectric Power
   
The final model selected is a **Generalized Additive Model (GAM)**, which best captures the non-linear relationships in the dataset.

## Research Question
Looking at the impact of different renewable sources on the total renewable energy consumption in the U.S. from 1980 to 2021, can the growth in total renewable energy consumption be explained by the combined influence of solar, wind, biomass, and hydroelectric energy?

### Hypotheses
- **Null Hypothesis (H₀)**: Solar, wind, biomass, and hydroelectric energy do not significantly impact total renewable energy consumption.
- **Alternative Hypothesis (H₁)**: At least one of the predictors significantly impacts total renewable energy consumption.

## Features
- ### Data Preparation & Cleaning:
  - Removed unnecessary columns, keeping only relevant energy sources.
  - Checked for missing values and ensured data integrity.
  - Filtered data for years 1980-2021.
  - Handled zero and non-positive values by filtering them out.
  - Applied log-transformation to address heteroscedasticity.

- ### Exploratory Data Analysis (EDA):
  - **Time-series plots** to visualize energy consumption trends.
  - **Correlation analysis** to identify relationships between predictors.
  - **Principal Component Analysis (PCA)** for dimensionality reduction.
  - **Pair plots & heatmaps** to analyze feature interactions.

- ### Model Building:
  - **Multiple Linear Regression (MLR)** as a baseline model.
  - **Generalized Additive Model (GAM)** for non-linear relationships.
  - **Feature selection using VIF and AIC/BIC.**
  - **Added interaction terms** for Solar × Wind Energy.


# Unemployment Analysis and Prediction Project

## Overview
This project focuses on analyzing unemployment trends and predicting unemployment rates using machine learning models. The dataset includes various features such as region, area (urban/rural), estimated employment, and labor participation rates.

Key objectives:
- Analyze trends in unemployment rates over time.
- Explore regional and area-wise unemployment disparities.
- Build and evaluate machine learning models to predict unemployment rates.

---

## Dataset
The dataset contains the following key columns:
- **Date:** The date of record.
- **Region:** Geographical region.
- **Area:** Urban or rural classification.
- **Estimated Unemployment Rate (%):** The target variable.
- **Estimated Employed:** Estimated number of employed individuals.
- **Estimated Labour Participation Rate (%):** Labor participation rate.

---

## Steps Performed
1. **Data Cleaning and Preprocessing:**
   - Removed missing values and stripped whitespaces from column names and values.
   - Converted the `Date` column to datetime format.
   - Encoded categorical variables (`Region` and `Area`) using one-hot encoding.

2. **Data Visualization:**
   - Trend analysis of unemployment rates over time.
   - Comparison of average unemployment rates across regions.
   - Rural vs. urban unemployment rate analysis.
   - Correlation heatmap for key variables.

3. **Machine Learning Pipeline:**
   - Data was split into training and testing sets.
   - Models evaluated: Random Forest, Linear Regression, Support Vector Regressor.
   - Random Forest Regressor was selected as the best-performing model based on R² score.

4. **Model Evaluation:**
   - Performance metrics: RMSE and R².
   - Visualized actual vs. predicted values.

5. **Model Deployment:**
   - Saved the trained model as a `.pkl` file for future use.

---

## Key Findings
- Unemployment rates vary significantly across regions and between urban and rural areas.
- There is a notable correlation between labor participation rates and unemployment.

---

## Usage
### Prerequisites
- Python 3.x
- Required libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`, `pickle`

### Run the Project
1. Clone this repository:
   ```bash
   git clone <repository-url>
   cd unemployment-analysis
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt

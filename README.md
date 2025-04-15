# covid19-us-analysis

This project is focused on analyzing the spread, impact, and trends of the COVID-19 pandemic across the United States using real-world data from "Our World in Data". Through multiple statistical and machine learning tasks, we uncover key insights into the progression of the pandemic, healthcare strain, and future forecasting using historical indicators.

## Dataset
We use a cleaned subset of the OWID COVID-19 dataset specific to the United States, containing metrics such as:
- Daily new cases and deaths
- 7-day averages
- ICU and hospital patient counts
- Derived change rates for cases and deaths

---

##  Tasks Overview

### Task 1: Exploratory Data Analysis (EDA)
- Visualized trends in new cases, deaths, hospitalizations, and ICU strain over time
- Explored correlations among health indicators
- Identified patterns in pandemic waves and healthcare burden using line plots and heatmaps

### Task 2: Classification
- Predicted `hospitalization_need` (Low, Medium, High) using logistic regression and random forest classifiers
- Evaluated models with accuracy, macro-F1 score, and confusion matrices
- Identified most predictive features (e.g., ICU patient count, case change rate)

### Task 3: Regression
- Used linear regression and random forest regression to predict continuous ICU patient counts
- Evaluated models using Mean Squared Error (MSE) and R² score
- Random Forest outperformed Linear Regression, with tighter prediction bounds and higher explanatory power

### Task 4: Outlier Detection
- Identified anomalous values in key metrics using:
  - IQR method (boxplots)
  - Z-score method (histograms)
- Highlighted unexpected spikes and drops in ICU data and new case trends

### Task 5: Time Series Forecasting
- Applied Prophet model to forecast ICU patient counts 30 days into the future
- Visualized predictions and 95% confidence intervals
- Decomposed trend, weekly seasonality, and yearly seasonality

Before running, make sure you have all the Python libraries installed, which is given below

Install the packages through your terminal:
pip install pandas numpy matplotlib seaborn scikit-learn prophet

Make sure you have all the files in the folder containing:
"owid_covid_data_us_subset.csv", "01_EDA.ipynb", "02_Classification.ipynb", "03_Regression.ipynb", "04_Outlier.ipynb", and "05_Time-Series-Forecasting.ipynb"

You can start on the first file to review the task and then move onto the next.

From there you will just have to press Shift + Enter to run each cell and each of the cells
should run the code to generate the tables and execute the plot or just go ahead and click 'Run All'.

After that, all of the codes should be running and show all the needed plots and results.

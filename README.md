# 🚲 Bike Rental Demand Prediction | Capstone Project

## Overview

This project was completed as a capstone data analytics and machine learning project for **OZ Bikes**, a fictional bike rental company operating in Sydney, Australia. The company experienced a significant decline in demand during the COVID-19 lockdowns and sought to prepare for post-pandemic recovery by understanding the key drivers of bike rental demand. 

The objective of this project was to identify the variables that have the strongest relationship with customer demand and build a predictive model that can help management make data-driven decisions to improve business performance and support future growth. 

---

## Business Problem

During the COVID-19 pandemic, OZ Bikes suffered financial losses due to reduced demand caused by lockdown restrictions. As restrictions were expected to ease, the company wanted to understand:

- Which factors influence bike rental demand the most
- How future demand can be predicted
- What business strategies could maximize bookings and profitability

The project focused on leveraging historical rental data to uncover actionable insights for operational planning and business growth. 

---

## Project Goals

The primary goal was to develop a machine learning model capable of predicting bike rental demand.

Specific objectives included:

- Performing exploratory data analysis (EDA)
- Identifying key demand drivers
- Building and evaluating a predictive model
- Generating business recommendations based on analytical findings

【1-6adc96】

---

## Dataset

The dataset contains:

- **730 observations**
- **16 variables**
- No missing values
- No significant outliers

Key variables include:

- Season
- Month
- Holiday
- Working Day
- Weather Situation
- Temperature
- Humidity
- Windspeed
- Bike Rental Count (`cnt`)



---

## Tools & Technologies

### Programming Language
- Python

### Environment
- Jupyter Notebook

### Libraries
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels

---

## Methodology

### 1. Data Preparation

- Imported and inspected the dataset
- Verified data quality
- Created dummy variables for categorical features
- Converted boolean values for modeling



### 2. Exploratory Data Analysis (EDA)

Boxplots and visualizations were used to explore relationships between bike rental demand and categorical variables such as:

- Season
- Month
- Weather Conditions
- Holidays
- Weekdays
- Working Days

Key findings showed that:

- Warmer months generated higher demand
- Favorable weather conditions increased usage
- Working days generally experienced higher rental volumes



### 3. Feature Engineering

- Generated dummy variables
- Split data using a 70:30 train-test ratio
- Applied feature scaling to prevent data leakage



### 4. Model Development

A Multiple Linear Regression model was built and refined through iterative feature selection.

Variables with:

- High Variance Inflation Factors (VIF)
- High p-values

were removed to reduce multicollinearity and improve model performance.

Several model iterations were performed before arriving at the final model. 

### 5. Predictive Modeling

The final model was used to predict demand on unseen test data and evaluate performance using:

- R² (R-Squared)
- Adjusted R²


---

## Key Findings

### Top Variables Influencing Bike Rental Demand

#### 1. Temperature (`temp`)
Coefficient: **0.5636**

A one-unit increase in temperature corresponds to an increase in bike rental demand, making temperature the strongest positive predictor. 【1-6adc96】

#### 2. Adverse Weather Conditions (`weathersit_3`)
Coefficient: **-0.3070**

Poor weather conditions significantly reduce bike rental demand. 

#### 3. Year (`yr`)
Coefficient: **0.2308**

Demand increased year-over-year, indicating growing customer adoption and market expansion. 

### Other Important Variables

- Season 4 (Winter) → Positive impact
- Windspeed → Negative impact


---

## Business Recommendations

### 🌡️ Optimize Promotions During Favorable Weather

- Increase advertising spend during warmer periods
- Launch seasonal campaigns when demand is naturally higher

### 🌦️ Weather-Responsive Strategies

- Offer incentives during poor weather
- Consider providing weather-friendly rider accessories

### 📈 Plan for Long-Term Growth

- Increase fleet capacity annually
- Expand infrastructure in high-demand locations

### ❄️ Seasonal Marketing Campaigns

- Introduce winter-focused promotions
- Partner with local businesses to create bundled offers

【1-6adc96】

---

## Results

The final machine learning model successfully identified the strongest drivers of bike rental demand and provided actionable business insights that can support:

- Demand forecasting
- Resource allocation
- Marketing optimization
- Strategic planning
- Business growth initiatives


---

## Repository Structure

```text
├── data/
│   └── bike_rental.csv
│
├── notebooks/
│   └── bike_rental_analysis.ipynb
│
├── images/
│   ├── boxplots.png
│   ├── correlation_matrix.png
│   └── prediction_results.png
│
├── presentation/
│   └── Bike Rental Business - Capstone.pdf
│
├── requirements.txt
│
└── README.md
```

---

## Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Statistical Analysis
- Data Visualization
- Multicollinearity Analysis (VIF)
- Linear Regression Modeling
- Predictive Analytics
- Business Intelligence
- Data-Driven Decision Making

---

## Author

**Ben Valencia**

Data Analytics & Machine Learning Portfolio Project

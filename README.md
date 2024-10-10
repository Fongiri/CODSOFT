# CODSOFT
## Repo for codsoft projects
# Sales Prediction Project

## Overview
This project implements a machine learning model to predict sales performance based on advertising spending across different media channels—TV, Radio, and Newspaper. By utilizing linear regression, we analyze the impact of these advertising efforts on sales conversion.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Results](#results)
- [Model Coefficients](#model-coefficients)
- [Conclusion](#conclusion)


## Introduction
Sales prediction is vital for businesses to formulate effective marketing strategies and optimize budgets. This project focuses on building a linear regression model to predict sales from advertising expenditures, helping drive informed decision-making.



## Dataset

The dataset used for this project is sourced from Kaggle and can be found at the following link: [Advertising Dataset](https://www.kaggle.com/datasets/ashydv/advertising-dataset).

### Dataset Overview

The Advertising dataset contains historical sales data and advertising expenditures across three media channels: TV, Radio, and Newspaper. Each row in the dataset represents a different observation that includes:

- **Sales:** The sales outcome for a given period.
- **TV:** The amount spent on television advertising in thousands of dollars.
- **Radio:** The amount spent on radio advertising in thousands of dollars.
- **Newspaper:** The amount spent on newspaper advertising in thousands of dollars.

### Data Description and Structure

| Column        | Description                                     |
|---------------|-------------------------------------------------|
| `Sales`      | The sales achieved in thousands of dollars.     |
| `TV`         | Advertising spend on TV in thousands of dollars. |
| `Radio`      | Advertising spend on Radio in thousands of dollars. |
| `Newspaper`   | Advertising spend on Newspaper in thousands of dollars. |

### Data Source

- **Source:** The dataset is publicly available on Kaggle and can be accessed at the following link: [Advertising Dataset](https://www.kaggle.com/datasets/ashydv/advertising-dataset).

### Usage

This dataset was analyzed using Python and relevant libraries (Pandas, NumPy, Scikit-learn) for data processing and linear regression modeling to predict sales based on advertising spend. Visualizations were created to better understand the relationships between advertising expenditure across different media channels and sales performance.

### Additional Notes

This dataset is essential for building a regression model aimed at providing insights into how different marketing channels impact sales outcomes, helping businesses allocate their advertising budgets more effectively.

## Methodology
1. **Data Preprocessing**
   - The dataset is loaded and inspected for missing values.
   - Features and target variables are defined as follows:
     - **Features (X):** TV, Radio, Newspaper
     - **Target Variable (y):** Sales

2. **Exploratory Data Analysis (EDA)**
   - A correlation matrix is created to understand relationships between features and sales.
   - Visualization through a heatmap using Seaborn helps to identify potential correlations between variables.

3. **Model Development**
   - The dataset is split into training and testing sets using an 80-20 ratio.
   - A linear regression model is trained on the training set.

4. **Model Evaluation**
   - Predictions are made on the test set.
   - Performance of the model is assessed using:
     - **Mean Squared Error (MSE)**
     - **R² Score**

5. **Residual Analysis**
   - Distribution of residuals is plotted to analyze prediction errors.

## Results
- **Mean Squared Error (MSE):** 3.00 
  - The average squared difference between the actual and predicted sales is 3.
  
- **R² Score:** 0.89 
  - Approximately 88.9% of the variance in sales is explained by the model, indicating a good fit.

## Model Coefficients
The coefficients derived from the linear regression model are as follows:

| Advertising Medium | Coefficient |
|--------------------|-------------|
| TV                 | 0.053860    |
| Radio              | 0.128354    |
| Newspaper          | -0.006290   |

### Fitted Model Equation
The regression equation derived from the model is: Sales = 4.07 + 0.05 * TV + 0.13 * Radio - 0.01 * Newspaper


**Interpretation:**
- For each additional unit (thousand dollars) spent on TV advertising, sales increase by approximately 0.054 units (thousand units).
- Each additional unit spent on Radio advertising results in an increase of about 0.128 units (thousand units) in sales, indicating a stronger impact than TV.
- The negative coefficient for Newspaper suggests that spending on this medium may not be effective, or could even detract from sales.

## Conclusion
The linear regression model effectively predicts sales based on advertising expenditures. The notable positive impact of Radio advertising suggests that businesses should consider reallocating resources towards effective channels. Further improvements could involve using advanced models or integrating additional variables for increased prediction accuracy.



---

Feel free to explore, modify, and contribute to this repository to enhance the prediction model further!

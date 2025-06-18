# Sales Prediction using Linear Regression

## Project Overview

This project aims to build a regression model to predict future sales based on historical data. The primary goal is to assist businesses in estimating future sales performance. The project involves data loading, preprocessing, handling missing values and outliers, feature engineering, data splitting, model training using Linear Regression, model evaluation, and data visualization.

## Task

Businesses struggle to estimate future sales based on past performance. This project addresses this problem by developing a regression model to predict future sales using historical data.

## Objective

Build a regression model to predict future sales using historical data.

## Requirements

- Use a CSV file with sales data (date, product, quantity, revenue).
- Preprocess the data and handle null values.
- Apply Linear Regression for modeling.
- Plot actual vs predicted sales.

## Expected Outcome

Graphical and tabular forecasts for upcoming sales periods.

## Dataset

The dataset used for this project is "sales_data.csv".

## Notebook Structure

The Jupyter Notebook is structured into the following sections:

1.  **Data loading:** Imports necessary libraries and loads the "sales_data.csv" file into a pandas DataFrame.
2.  **Data cleaning:** Checks for and handles potential missing values. Identifies outliers using Z-scores and IQR methods.
3.  **Data wrangling:** Aggregates the sales data by date to get total daily revenue, preparing the data for time series analysis.
4.  **Feature engineering:** Creates time-based features (year, month, day of the week) from the date column.
5.  **Data splitting:** Splits the data into training and testing sets based on time, ensuring the testing set contains later dates.
6.  **Model training:** Trains a Linear Regression model on the training data.
7.  **Model evaluation:** Evaluates the performance of the trained Linear Regression model on the testing data using MAE, MSE, and R-squared metrics.
8.  **Data visualization:** Plots the actual sales from the testing set against the predicted sales to visually assess the model's performance.
9.  **Summary:** Provides a summary of the key findings from the data analysis and model evaluation, along with insights and potential next steps.

## Key Findings

- The dataset contains 10,000 entries with columns including `OrderID`, `Product`, `Category`, `Region`, `Quantity`, `PricePerUnit`, `TotalSales`, and `Date`.
- No missing values were found.
- Outliers were identified in numerical columns.
- Daily total revenue was calculated and time-based features were engineered.
- The data was split into training (80%) and testing (20%) sets chronologically.
- The Linear Regression model trained on the data performed poorly, as indicated by a negative R-squared score and high MAE and MSE values.

## Next Steps

- Investigate more advanced time series models (e.g., ARIMA) or other regression techniques.
- Explore additional feature engineering possibilities (e.g., lag features, moving averages, holiday indicators).
- Address the identified outliers in the original data, potentially using capping, removal, or transformation methods.
- Consider robust regression techniques that are less sensitive to outliers.

## How to Run the Notebook

1.  Ensure you have Jupyter Notebook or Google Colab installed.
2.  Download the "sales_data.csv" file and place it in the same directory as the notebook, or upload it to your Colab environment.
3.  Open the notebook in Jupyter Notebook or Colab.
4.  Run the cells sequentially to execute the code.

## Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- sklearn

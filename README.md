# Quality of Life Index Analysis

## Overview
This program looks at the relationship between different economic and social factors and **Quality of Life Index** across different countries. It uses **linear regression** to predict the Quality of Life Index based on some of the key factors.

## Steps in the Program

1. **Load Data**
   - Read the data (`quality_of_life_indices_by_country.csv`) with Pandas
   - Select relevant columns for analysis

2. **Data Exploration**
   - Checks for correlation between the different factors
   - Visualize relationships using Seaborn (`lmplot`) and histogram plots

3. **Training and Testing**
   - Split the dataset into training (`train`) and testing (`test`) sets
   - Training data: Rows **1 to 1196**
   - Testing data: Rows **after 1196**

4. **Train the Model**
   - Use LinearRegression to train a model, using the following predictors:
     - **Purchasing Power Index**
     - **Safety Index**
     - **Health Care Index**
     - **Cost of Living Index**
     - **Property Price to Income Ratio**
   - Fit the model on the training set

5. **Make Predictions**
   - Predict Quality of Life Index for the test set
   - Round predictions to 2 decimal places

6. **Evaluate Model Performance**
   - Compute **Mean Absolute Error** between actual and predicted values
   - Compare the mean absolute error with the standard deviation of the quality of life index

## Possible Improvements
- I'm no expert with ML, so there are definitely ways to improve upon this model
- **Non-Linear** models for example may result in closer prediction than reached here

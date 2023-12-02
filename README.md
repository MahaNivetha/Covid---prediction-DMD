# Covid---prediction-DMD

# DMD Analysis Code README

## Overview

This MATLAB code performs Dynamic Mode Decomposition (DMD) analysis on COVID-19 data. DMD is used to predict the future cases and analyze the system's dynamic behavior. The code allows for both automatic analysis of DMD with pre-defined parameters and interactive prediction of cases within or beyond the input window.

## Usage Instructions

1. **Data Input:**
   - The code reads COVID-19 data from a CSV file named `cov2.csv`. Ensure the file is in the correct format.

2. **Automatic DMD Analysis:**
   - Choose option 1 to perform the analysis of DMD automatically with pre-defined parameters.
   - The code provides three cases with different parameters:
      - Case 1: Rank 10, Input Window 100, Prediction 3.
      - Case 2: Rank 10, Input Window 300, Prediction 60.
      - Case 3: Rank 35, Input Window 100, Prediction 20.
   - The code generates plots for actual vs. predicted cases, discrete and continuous-time eigenvalues, and error metrics (RMSE, MSE, MAE).

3. **Interactive Prediction:**
   - Choose option 2 to use interactive prediction of cases.
   - Select whether to predict within the input window or into the future.
   - Specify the number of states to observe for comparison.
   - If predicting into the future, enter the number of days to predict.
   - The code generates plots for actual vs. predicted cases and eigenvalues.
   - For future prediction, the code also provides scatter plots for better visualization.

## Functions

1. **DMD Function:**
   - The `DMD` function performs Dynamic Mode Decomposition on the input data.
   - It returns eigenvalues, continuous-time eigenvalues, and predicted cases.
   - The function accepts parameters like the starting point, maximum columns, prediction length, rank, time interval, and number of days to predict.

2. **Error Metrics:**
   - The `rmse`, `mse`, and `mae` functions calculate Root Mean Square Error, Mean Squared Error, and Mean Absolute Error, respectively.


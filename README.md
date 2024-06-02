# Covid19-prediction-using-dmd
This MATLAB project analyzes and predicts COVID-19 cases using Dynamic Mode Decomposition (DMD). It includes functionalities for interactive prediction of cases and various analysis cases with different parameters. The code also features random selection of states for plotting actual vs. predicted cases to provide diverse visual insights. The project is structured to provide two primary functionalities:
- Analysis of DMD on COVID-19 Data
- Interactive Prediction of COVID-19 Cases

## Usage
Run the script: Execute the MATLAB script to start the analysis.

User Input: The script prompts the user for input to choose between analysis or interactive prediction.

- Enter 1: Perform analysis using DMD.
- Enter 2: Use interactive prediction to forecast future COVID-19 cases.
### Analysis of DMD (Option 1)
When the user selects analysis:

- Case 1: Rank 10, Number of columns for X: 100, Prediction: 3 days.
- Case 2: Rank 10, Number of columns for X: 300, Prediction: 60 days.
- Case 3: Rank 35, Number of columns for X: 100, Prediction: 20 days.

The analysis involves:

- Calculating and plotting the actual vs predicted cases.
- Plotting the discrete and continuous-time eigenvalues.
- Calculating RMSE, MSE, and MAE for the predicted values.
- Performing analysis on states and evaluating errors.

### Interactive Prediction of Cases (Option 2)
When the user selects interactive prediction:

Input Window Prediction: Predict within the input window for easy comparison.

Future Prediction: Predict the cases for a specified number of future days.
The interactive prediction involves:

- Displaying the RMSE of the predicted values.
- Plotting actual vs predicted cases for each state.
- Plotting predicted cases for future days using scatter plots.

## Functions
- DMD(Xaug, start, m, l, r, dt, n1): Computes the Dynamic Mode Decomposition and returns the eigenvalues and predictions.
- rmse(a, b): Computes the Root Mean Square Error.
- mse(a, b): Computes the Mean Square Error.
- mae(a, b): Computes the Mean Absolute Error.

## Dataset
The dataset initially contained 3,667,271 records spanning 56 states over 1,086 days. After substantial preprocessing, it was reduced to 61,959 records by combining data from all states into a unified representation and narrowing the focus.

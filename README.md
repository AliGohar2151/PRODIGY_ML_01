# House Price Prediction using Linear Regression

This project demonstrates a simple linear regression model to predict house prices using features such as above-ground living area, number of bedrooms above ground, and the number of full bathrooms. The model is trained on a dataset provided in CSV format.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Code Explanation](#code-explanation)
  - [Patch 1: Import Libraries and Load Data](#patch-1-import-libraries-and-load-data)
  - [Patch 2: Select Features and Handle Missing Values](#patch-2-select-features-and-handle-missing-values)
  - [Patch 3: Train the Linear Regression Model](#patch-3-train-the-linear-regression-model)
  - [Patch 4: Make Predictions and Save the Results](#patch-4-make-predictions-and-save-the-results)
- [Output](#output)

## Prerequisites

- Python 3.x
- Jupyter Notebook
- Required Python libraries: `pandas`, `scikit-learn`
- Dataset : https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data

## Installation

1. Clone this repository to your local machine.
2. Install the required libraries using the following command:

    ```bash
    pip install pandas scikit-learn
    ```

3. Open the Jupyter Notebook and navigate to the project directory.

## Usage

Follow these steps to use the code in a Jupyter Notebook:

1. **Patch 1**: Import the necessary libraries (`pandas`, `scikit-learn`) and load the training and testing datasets from CSV files. Display the first few rows to understand the data structure.
2. **Patch 2**: Select relevant features (like `GrLivArea`, `BedroomAbvGr`, `FullBath`) from the training data that will be used to predict the target variable (`SalePrice`). Handle any missing values by filling them with the mean.
3. **Patch 3**: Initialize and train a linear regression model using the selected features from the training data.
4. **Patch 4**: Use the trained model to predict house prices for the test dataset. Save the predicted results to a CSV file named `house_price_predictions.csv`.

Run these patches step-by-step to complete the model training and prediction process.

## Code Explanation

### Patch 1: Import Libraries and Load Data

- **Objective**: Import necessary libraries and load the datasets.
- **Instructions**: Run this patch to load the `train.csv` and `test.csv` files into the notebook and inspect the data.

### Patch 2: Select Features and Handle Missing Values

- **Objective**: Select features and target variable for training, and handle missing values.
- **Instructions**: Run this patch to select the relevant features and handle any missing values in both training and test datasets.

### Patch 3: Train the Linear Regression Model

- **Objective**: Train a linear regression model using the selected features.
- **Instructions**: Run this patch to initialize the model, train it using the training data, and fit the model.

### Patch 4: Make Predictions and Save the Results

- **Objective**: Predict house prices for the test dataset and save the results.
- **Instructions**: Run this patch to make predictions using the trained model and save them to `house_price_predictions.csv`.

## Output

- The predictions will be saved to a file named `house_price_predictions.csv` in the current directory.
- The CSV file will contain the house IDs and the predicted sale prices.

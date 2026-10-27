# Bike Rental Prediction with Regression

A two-part machine learning lab that explores a daily bike-share dataset and trains regression models to predict the number of bike rentals per day.

## Labs

### Lab 1: Linear Regression
`Bike_Rental_Regression_Lab.ipynb`

A complete beginner-friendly regression workflow:

1. **Load the data** – read the daily bike-share CSV into a pandas DataFrame.
2. **Explore the data** – summarize numeric features and visualize their distributions.
3. **Analyze relationships** – compare each feature (numeric and categorical) with the number of rentals.
4. **Prepare the data** – separate features from the label and split into training (70%) and test (30%) sets.
5. **Train the model** – fit a Linear Regression model with scikit-learn.
6. **Evaluate the model** – compare predictions to actual values using MSE, RMSE, and R².

### Lab 2: Experimenting with Additional Models
`Experimenting_Additional_Models_Lab.ipynb`

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/maramadel6789-web/bike-rental-regression/blob/main/Experimenting_Additional_Models_Lab.ipynb)

Builds on Lab 1 by training and comparing more regression algorithms on the same data:

- **Lasso** – a linear model variant
- **Decision Tree** – a tree-based model
- **Random Forest** – an ensemble that averages many decision trees (bagging)
- **Gradient Boosting** – an ensemble that builds trees sequentially to reduce error (boosting)

Each model is evaluated using MSE, RMSE, and R², with a plot of predicted vs. actual rentals.

## Dataset

`daily-bike-share.csv` contains one row per day, with the following main columns:

| Column | Description |
|---|---|
| `season`, `mnth`, `weekday` | Time-related features |
| `holiday`, `workingday` | Day type |
| `weathersit` | Weather situation category |
| `temp`, `atemp`, `hum`, `windspeed` | Normalized weather measurements |
| `rentals` | **Label** – number of bikes rented that day |

## Requirements

- Python 3
- pandas
- numpy
- matplotlib
- scikit-learn

Install them with:

```bash
pip install pandas numpy matplotlib scikit-learn
```

## How to Run

1. Clone or download this repository.
2. Make sure `daily-bike-share.csv` is in the same folder as the notebooks.
3. Open a notebook in Jupyter Notebook, JupyterLab, or Google Colab (if using Colab, upload `daily-bike-share.csv` to the session first).
4. Run the cells from top to bottom.

## Evaluation Metrics

- **MSE** (Mean Squared Error) – average of the squared prediction errors.
- **RMSE** (Root Mean Squared Error) – square root of the MSE, in the same units as the label (rentals).
- **R²** (Coefficient of Determination) – how much of the variation in rentals the model explains.

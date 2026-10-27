# bike-rental-regression
Predicting daily bike rentals using linear regression
# Bike Rental Prediction with Linear Regression

A machine learning lab that explores a daily bike-share dataset and trains a linear regression model to predict the number of bike rentals per day.

## Overview

The notebook walks through a complete beginner-friendly regression workflow:

1. **Load the data** – read the daily bike-share CSV into a pandas DataFrame.
2. **Explore the data** – summarize numeric features and visualize their distributions.
3. **Analyze relationships** – compare each feature (numeric and categorical) with the number of rentals.
4. **Prepare the data** – separate features from the label and split into training (70%) and test (30%) sets.
5. **Train the model** – fit a Linear Regression model with scikit-learn.
6. **Evaluate the model** – compare predictions to actual values and measure performance with MSE, RMSE, and R².

## Dataset

`daily-bike-share.csv` contains one row per day, with the following main columns:

| Column | Description |
|---|---|
| `season`, `mnth`, `weekday` | Time-related features |
| `holiday`, `workingday` | Day type |
| `weathersit` | Weather situation category |
| `temp`, `atemp`, `hum`, `windspeed` | Normalized weather measurements |
| `rentals` | **Label** – number of bikes rented that day |

## Repository Contents

- `Bike_Rental_Regression_Lab.ipynb` – the lab notebook, with a short explanation above each code cell
- `daily-bike-share.csv` – the dataset

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
2. Make sure `daily-bike-share.csv` is in the same folder as the notebook.
3. Open the notebook in Jupyter Notebook, JupyterLab, or Google Colab.
4. Run the cells from top to bottom.

## Evaluation Metrics

- **MSE** (Mean Squared Error) – average of the squared prediction errors.
- **RMSE** (Root Mean Squared Error) – square root of the MSE, in the same units as the label (rentals).
- **R²** (Coefficient of Determination) – how much of the variation in rentals the model explains.

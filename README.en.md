[🇧🇷 Português](README.md) · 🇺🇸 **English**

# Regression model for marketing spend

A model that estimates sales from spend on YouTube, Facebook, and newspaper ads, to support decisions about where to put the budget.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/guilhsantos/Modelo_de_Regressao_para_Marketing/blob/main/Modelo_de_Regress%C3%A3o_para_Marketing.ipynb)

## Problem

The company invests in three media channels every month, but doesn't know how much each one contributes to sales or what return to expect from a new spending plan.

## Solution

A linear regression trained on historical spend and sales (`MKT.csv`) that takes a media plan and returns the predicted sales.

## Result

On the test set (20% of the data):

| Metric | Value |
|---|---|
| **R²** | **0.87**: the model explains 87% of the variation in sales |
| RMSE | 2.36 (in the dataset's sales unit) |
| MSE | 5.58 |

The notebook ends with a simulator: you enter the spend per channel and get the predicted sales.

## How I did it

1. **Descriptive analysis:** structure, nulls, and statistics for each channel.
2. **Exploratory analysis:** pairplot and correlation matrix between spend and sales.
3. **Modeling:** linear regression (scikit-learn) with an 80/20 train/test split.
4. **Evaluation:** MSE, RMSE, R², and an actual vs. predicted plot.
5. **Prediction:** test with new spend values.

## Next steps

- Read the coefficients to say how much each extra unit of spend per channel returns in sales.
- Test channel interactions and diminishing returns, since doubling spend rarely doubles sales.

## Stack

Python · pandas · NumPy · scikit-learn · Seaborn · Matplotlib · Google Colab

---

Made by [Guilherme Santos](https://portifolio-guilherme-santos.vercel.app) · [LinkedIn](https://www.linkedin.com/in/guilherme-santos-dataeng)

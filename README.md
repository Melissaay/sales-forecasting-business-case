# Sales Forecasting for S&OP

## Context

This project is inspired by the implementation of a sales forecasting process in a complex B2B environment.

Forecasting in this context is not only a statistical problem:
- evolving product ranges (new vs old generations)
- irregular demand patterns
- operational constraints
- need for business-usable outputs

---

## Objective

Develop a forecasting approach that produces reliable and usable sales predictions to support S&OP decision-making.

---

## Data

The dataset used in this project is synthetic and created for demonstration purposes.

It reproduces realistic business patterns (seasonality, product lifecycle, demand variability) inspired by real-world use cases.

No confidential or company data is used.

---

## Approach

The forecasting approach combines time series modeling with business-specific adjustments:

- aggregation of sales data at product level
- handling of product substitutions (old → new references)
- integration of working days as a business driver
- inclusion of holidays effects (France)
- evaluation of model performance using multiple metrics

---

## Model

The model is based on Prophet, adapted to fit business constraints.

It relies on an additive decomposition of time series:

y(t) = trend + seasonality + holidays + regressors + error

Key elements:

- **Trend**: captures long-term evolution of sales  
- **Seasonality**: yearly patterns in demand  
- **Holidays**: impact of national holidays  
- **Regressors**: integration of business variables (e.g. working days)  

The goal is not only accuracy, but interpretability and usability.

---

## Key business features

This project goes beyond standard forecasting:

- product substitution logic to reflect real product lifecycle
- integration of working days as an operational driver
- alignment with business understanding of sales dynamics

---

## Evaluation

Model performance is evaluated using:

- MAPE  
- RMSE  
- MAE  

Results are analyzed through:

- comparison between actual and predicted sales
- aggregated performance across multiple products

---

## Results

- the model provides coherent forecasts across several product lines
- simple business variables (e.g. working days) improve predictions
- forecasts are interpretable and usable for planning

---

## Key takeaway

In a business context, a good forecasting model is not only about accuracy.

It must:
- reflect real-world constraints
- integrate business logic
- produce outputs that can support decision-making

---

## Tech stack

Python · Pandas · Prophet · Time series modeling · Data preprocessing · Visualization

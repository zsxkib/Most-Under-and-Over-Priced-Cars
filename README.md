# Most Under/Over Priced Cars

#### The task is to determine what influences and drives the car prices given its technical specs. Specifically, which car(s) I believe to be most under/overpriced and why.

## Overview

_**This was a take-home assignment for a Graduate Data Analyst Consultant position at a Machine Learning Consultancy**_

Within the repo you will find the following:
*	car_data_cleaned.csv 
> (Raw data .csv file sent by the Machine Learning Consultancy)
*	code.(pdf/html)
> PDF (.pdf) & Web (.html) versions of my notebook, just in case there’s technical difficulties with original Jupyter notebook)
*	code.ipynb 
> (Jupyter Notebook containing all analysis, code, plots, etc)
*	method_results_conclusion.pptx 
> Three slide presentation outlining method, results, and conclusion)

## Method

* Exploratory Data Analysis
* Clean Data
* XGBoost Regressor with 5-Fold Cross-Validation
* Under/Over-priced Car Ranking per Fold
* XGBoost Regressor on Top/Bottom 50 in Ranking
* SHapley Additive exPlanations (SHAP)

## Results

### Top 3 Most Over-Priced Cars:
![image](/plots/most_over_priced_car_and_why.png?raw=true "Top 3 Most Over-Priced Cars SHAP Force Plot")

* **2018 Mercedes-Benz G Class Specs: G550 4x4 Squared**
> True MSRP = 227 300
> Predicted MSRP = 120 390.77
> Ratio (True/Predicted) = 1.888

* 2019 Jaguar XE SV Specs: Project 8 AWD
> True MSRP = 187 500
> Predicted MSRP = 119 680.59
> Ratio (True/Predicted) = 1.566

* 2018 Porsche 911 Specs: GT2 RS Coupe
>True MSRP = 293 200
>Predicted MSRP = 193 417.28
> Ratio (True/Predicted) = 1.515


### Top 3 Most Under-Priced Cars
![image](/plots/most_under_priced_car_and_why.png?raw=true "Top 3 Most Under-Priced Cars SHAP Force Plot")

* **2018 Jeep Grand Cherokee Specs: Altitude 4x4**
> True MSRP = 33 195
> Predicted MSRP = 47 957.96
> Ratio (True/Predicted) = 0.692

* 2018 Jeep Grand Cherokee Specs: Upland 4x4
> True MSRP = 33 195
> Predicted MSRP = 47 957.96
> Ratio (True/Predicted) = 0.692

* 2019 Dodge Challenger Specs: R/T Scat Pack Widebody RWD
> True MSRP = 38 995
> Predicted MSRP = 56 335.17
> Ratio (True/Predicted) = 0.692

![image](/plots/why.png?raw=true "Most Under/Over-Priced Cars SHAP Waterfall Plots")

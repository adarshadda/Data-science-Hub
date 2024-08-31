# Customer Churn Predictions for PowerCo

This project involves predicting customer churn for PowerCo, a major gas and electricity utility. The goal is to identify factors contributing to customer churn and build predictive models to help PowerCo improve retention.

## Project Overview

### Background
PowerCo is facing increased competition in the energy market, leading to higher customer churn rates. To address this, BCG has been engaged to diagnose the reasons behind customer churn and develop strategies for improvement.

### Data Description
The dataset consists of customer-related information and includes the following types of data:

- **Customer Data**: Characteristics such as industry, historical electricity consumption, and date joined.
- **Churn Data**: Indicates whether a customer has churned.
- **Historical Price Data**: Details on prices charged to customers for electricity and gas at granular intervals.

### Data Columns
The dataset contains 26 columns:

| #  | Column                          | Non-Null Count | Dtype  |
|----|---------------------------------|----------------|--------|
| 0  | id                              | 14606          | object |
| 1  | channel_sales                   | 14606          | object |
| 2  | cons_12m                        | 14606          | int64  |
| 3  | cons_gas_12m                    | 14606          | int64  |
| 4  | cons_last_month                 | 14606          | int64  |
| 5  | date_activ                      | 14606          | object |
| 6  | date_end                        | 14606          | object |
| 7  | date_modif_prod                 | 14606          | object |
| 8  | date_renewal                    | 14606          | object |
| 9  | forecast_cons_12m               | 14606          | float64|
| 10 | forecast_cons_year              | 14606          | int64  |
| 11 | forecast_discount_energy        | 14606          | float64|
| 12 | forecast_meter_rent_12m         | 14606          | float64|
| 13 | forecast_price_energy_off_peak  | 14606          | float64|
| 14 | forecast_price_energy_peak      | 14606          | float64|
| 15 | forecast_price_pow_off_peak     | 14606          | float64|
| 16 | has_gas                         | 14606          | object |
| 17 | imp_cons                        | 14606          | float64|
| 18 | margin_gross_pow_ele            | 14606          | float64|
| 19 | margin_net_pow_ele              | 14606          | float64|
| 20 | nb_prod_act                     | 14606          | int64  |
| 21 | net_margin                      | 14606          | float64|
| 22 | num_years_antig                 | 14606          | int64  |
| 23 | origin_up                       | 14606          | object |
| 24 | pow_max                         | 14606          | float64|
| 25 | churn                           | 14606          | int64  |


## Exploratory Data Analysis (EDA)

The EDA phase involved analyzing data distributions, detecting correlations, and understanding data characteristics. Key findings include:

- **Price Fluctuations**: The impact of price changes on customer churn.
- **Consumption Patterns**: How historical consumption and forecasted consumption affect churn.
- **Categorical Data**: Encoding of categorical variables for model training.

## Feature Engineering & Modeling

### Price Change Features

- **Difference in Prices**: Calculated the difference between off-peak prices in December and the preceding January.
- **Average Price Changes**: Created features reflecting average price changes across different periods.
- **Max Price Changes**: Included maximum price changes between months and periods.

### Data Transformation

- **Categorical Data**: Used one-hot encoding to convert categorical features into numerical form.
- **Numerical Data**: Applied logarithmic transformation to address skewness in continuous variables.

### Data Sampling

- Split the dataset into training (75%) and testing (25%) sets to evaluate model performance.

## Model Results

- **Random Forest Model**: Demonstrated strong predictive power for non-churning customers but struggled with accurately predicting churn due to class imbalance.
- **Key Predictors**: The most influential predictors of churn include past energy consumption, forecasted meter rental costs, and the company's net margin.


## Conclusion

The most influential predictors of churn include:

- **Past Energy Consumption** (`cons_12m`)
- **Predicted Meter Rental Costs** (`forecast_meter_rent_12m`)
- **Net Margin from Customers** (`net_margin`)

These factors highlight the importance of pricing, cost transparency, and customer profitability in retention efforts. Customers' past consumption behavior, expected meter rental costs, and the company's net margin play significant roles in their decision to churn. Additionally, variables related to energy prices, consumption patterns, and contract details are also important in predicting churn.



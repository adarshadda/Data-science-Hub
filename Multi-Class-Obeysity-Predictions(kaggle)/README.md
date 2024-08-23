## Project Overview
The data consist of the estimation of obesity levels in people from the countries of Mexico, Peru and Colombia, with ages between 14 and 61 and diverse eating habits and physical condition , data was collected using a web platform with a survey where anonymous users answered each question, then the information was processed obtaining 18 attributes and 20758 records.

The data contains numerical data and continous data, so it can be used for analysis based on algorithms of classification, prediction, segmentation and association. Data is available in CSV format

## Objectives

1. **Predict Obesity Levels**: Develop and evaluate predictive models to classify individuals into categories such as Insufficient Weight, Normal Weight, Overweight, and various Obesity Types.
2. **Identify Key Factors**: Analyze features to understand the most influential factors contributing to obesity. This can guide public health interventions and personalized health recommendations.

## About Dataset

This dataset encompasses data for the estimation of obesity levels in individuals from the countries of Mexico, Peru, and Colombia, based on their eating habits and physical condition. 

**Key Points:**

* **Records:** 20758
* **Attributes:** 18
* **Target Variable:** `NObesity` (Obesity Level)
* **Target Classes:** 
    * Insufficient Weight
    * Normal Weight
    * Overweight Level I
    * Overweight Level II
    * Obesity Type I
    * Obesity Type II
    * Obesity Type III

**Attribute Details:**

1. `Gender` 
2. `Age`
3. `Height` 
4. `Weight` 
5. `family_history_with_overweight`
6. `FAVC`: Frequent consumption of high-calorie food 
7. `FCVC`: Frequency of consumption of vegetables 
8. `NCP`: Number of main meals per day 
9. `CAEC`: Consumption of food between meals
10. `SMOKE`: Smoker 
11. `CH2O`: Consumption of water daily 
12. `SCC`: Calories consumption monitoring 
13. `FAF`: Physical activity frequency per week 
14. `TUE`: Time using technology devices per day 
15. `CALC`: Consumption of alcohol 
16. `MTRANS`: Transportation used 
17. `NObesity`: TARGET Target variable 

**Note:**

* The dataset is suitable for various machine learning tasks, including classification, clustering, and regression, due to the mix of numerical and categorical data and the presence of a labeled target variable.



## Results

The XGBoost model achieved an accuracy of 91% in predicting obesity levels. The model was compared with other classifiers such as Random Forest and Logistic Regression, demonstrating superior performance in precision, recall, and F1-score.

### Feature Importance:

- **Gender_Female**: 0.255
- **Gender_Male**: 0.178
- **BMI**: 0.161
- **Weight**: 0.089
- **FAVC_yes**: 0.037
- **FCVC**: 0.035
- **SCC_yes**: 0.022
- **TUE**: 0.013
- **Family History_with_Overweight_yes**: 0.014
- **FAF**: 0.009
- **SMOKE_yes**: 0.005

## Contributing

Feel free to contribute to this project by submitting issues or pull requests. For major changes, please open an issue first to discuss what you would like to change.


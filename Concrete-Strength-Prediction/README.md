# Modified Concrete Strength Prediction Using Machine Learning

Concrete strength prediction is essential in construction projects to ensure the material meets safety and performance standards. This project uses machine learning techniques to predict the compressive strength of hybrid concrete having silifa fume as partial replacement of cement, waste glass powder as partial substitute of sand and recycled aggregates as coarse aggregates. Also, the project involves predicting concrete compressive strength based on multiple features, such as water-to-binder ratio, superplasticizer content, and curing age (days).

## Datasets:

**Feature Variables:**

1. Cement_kg_m3
2. SilicaFume_%_of_cement_kg_m3
3. Sand_kg_m3
4. GlassPowder_%_of_sand_kg_m3
5. Recycled_Aggregate_kg_m3
6. Water_Binder_ratio
7. Superplasticizer_%_of_binder_kg_m3
8. Curing_Age_days

**Target Variable:**
1. fc_MPa_28d


## Models Used:
1. Linear Regression
2. Ridge Regression
3. Support Vector Machines
4. Decision Tree Regression
5. MLP Regression
6. Random Forest Regression
7. Gradient Boosting Regression
8. Ada Boost Regression

## Procedures:
**Data Preprocessing:** The dataset is preprocessed, with missing values handled and features standardized.
**Model Training:** Different machine learning models are trained on the preprocessed data.
**Evaluation:** Models are evaluated using metrics like R-squared, MSE, MAE and RMSE.
**Prediction:** The trained models are used to predict the compressive strength of new concrete mixes.
# Modified Concrete Strength Prediction Using Machine Learning

Concrete strength prediction is essential in construction projects to ensure the material meets safety and performance standards. This project uses machine learning techniques to predict the compressive strength of hybrid concrete having silifa fume as partial replacement of cement, waste glass powder as partial substitute of sand and recycled aggregates as coarse aggregates. Also, the project involves predicting concrete compressive strength based on multiple features, such as water-to-binder ratio, superplasticizer content, and curing age (days).

## Datasets:

**Feature Variables:**

* Cement_kg_m3
* SilicaFume_%_of_cement_kg_m3
* Sand_kg_m3
* GlassPowder_%_of_sand_kg_m3
* Recycled_Aggregate_kg_m3
* Water_Binder_ratio
* Superplasticizer_%_of_binder_kg_m3
* Curing_Age_days

**Target Variable:**
* fc_MPa_28d


## Models Used:
* Linear Regression
* Ridge Regression
* Support Vector Machines
* Decision Tree Regression
* MLP Regression
* Random Forest Regression
* Gradient Boosting Regression
* Ada Boost Regression

## Procedures:
* **Data Preprocessing:** The dataset is preprocessed, with missing values handled and features standardized.
* **Model Training:** Different machine learning models are trained on the preprocessed data.
* **Evaluation:** Models are evaluated using metrics like R-squared, MSE, MAE and RMSE.
* **Prediction:** The trained models are used to predict the compressive strength of new concrete mixes.
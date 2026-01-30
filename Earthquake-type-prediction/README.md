# Earthquake Type Prediction Using Deep Learning

Earthquake data analysis is essential for understanding seismic patterns and improving monitoring systems. This project uses machine learning—specifically a deep neural network—to predict whether an earthquake record is Reviewed or not based on multiple seismic and temporal features. The goal is to identify patterns in earthquake records and classify their review status using historical data.

## Datasets:
The dataset is collected from historical earthquake records and includes information related to time, magnitude, location, and data sources.

**Feature Variables:**

* Latitude
* Longitude
* Depth
* Magnitude
* Root Mean Square
* Year
* Month
* Hour
* Type (encoded)
* Magnitude Type (encoded)
* Source (encoded)
* Location Source (encoded)
* Magnitude Source (encoded)
* Other derived and encoded numerical features

**Target Variable:**

* Status:
1 → Reviewed
0 → Not Reviewed


## Models Used:
* Deep Neural Network (Artificial Neural Network) using TensorFlow/Keras

## Procedures:

**Data Preprocessing:**

* The dataset was loaded using Pandas.
* Columns with more than 66% missing values were removed.
* Missing values in the Root Mean Square column were filled with the mean.
* Rows with missing values in important fields (like Magnitude Type) were dropped.
* Irrelevant columns such as ID were removed.

**Feature Engineering:**

* Date and Time columns were split into: Month, Year, Hour
* Invalid year values containing non-numeric characters were removed.
* The Status column was converted into binary form:
1. Reviewed → 1
2. Otherwise → 0

**Data Visualization:**

* A correlation heatmap is used to observe relationships between numeric variables.
* KDE plots are used to understand feature distributions after standardization.
* Observations show that reviewed cases increase over the years.

**Encoding:**

Categorical variables such as:

* Type
* Magnitude Type
* Source
* Location Source
* Magnitude Source
were converted into numeric form using One-Hot Encoding.

**Feature Scaling:**

Standardization was applied using StandardScaler to normalize the feature values for better neural network performance.

**Train-Test Split:**

* 70% of data was used for training.
* 30% was used for testing.

* The dataset showed class imbalance:

1. ~89% Reviewed
2. ~11% Not Reviewed

**Model Training:**

* Optimizer : Adam
* Loss Function : Binary Crossentropy
* Metric : AUC
* Batch Size : 32
* Epochs : 30

**Evaluation:**

* Training and validation loss were plotted to monitor overfitting.
* AUC score was used to measure classification performance.
* Final evaluation was done using the test dataset.

**Prediction:**

The trained neural network model can classify new earthquake records as:

1. reviewed
2. automatic
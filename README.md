# Diabetes Prediction using Logistic Regression

In this project we try predict if a patient has diabetes or not depending on different health parameters using logistic regression.


## Apendix

- Part 1 - EDA - Visuals
    - Countplot of how many patients have diabetes.
    - Displot of Diabetic patient wrt age
    - Seeing the change of diabetes with no of pregnancy 
    - Histogram plot of Diabetic patient wrt age
    - Heatmap of correlation
    - Histplot of all features
    - Box Plot of Age vs BMI
    - KDE plot of Outcome (Diabetic) wrt numerical feature

- Part 2 - Model Building
    - Train TestSplit
    1) Logistic regression model
    - Confusion Matrix and Accruacy
    - Predicting
    - Seeing Feature Importance
    2) LightGBM model
    -  LGBMClassifier
    - gridsearch
    - Model Performance
    - Score table

## A beirf Info On dataset

The dataset consists of the following parameters.
Pregnancies,
Glucose,
BloodPressure,
SkinThickness,
Insulin,
BMI,
DiabetesPedigreeFunction,
Age

Using these features we pridict the outcome if diabetes is there or not.


## Part 1 _ visualization

We then Perform EDA on this.
Some key visualizations include
1) The countplot shows that 2/3 of people in our dataset doent have diabetis.

2) The displot shows that disbetes is more common in young age group and less common for older people.
The skewness was 1.12 and krutosis of 0.6

3) Seeing the change of diabetes with no of pregnancy 

4) Histogram plot of Diabetic patient wrt age
minimun age with diabetes = 21
q1 = 24
median = 29
q3 = 41
maximun age with diabetes = 66 with few outliers(6) of more than 66

4) Heatmap of correlation
we see that age and Glucose has higher correlation(0.5) for diabetes
followed by BMI (0.3)

5) Histplot of all features
Glucose , blood pressure and BMI have a normal distribution
Age , insulin and DiabetesPedigreeFunction are skewed

6) Box Plot of Age vs BMI
shows the variation of BMI for age 

7) KDE plot of Outcome (Diabetic) wrt numerical feature
the numeric features are 
'Pregnancies','Glucose','BloodPressure','SkinThickness','Insulin', 'BMI','DiabetesPedigreeFunction','Age'

## Part 2 - Model Building

### 1) Logistic Regression Model

- Accuracy = 79.1 %

- ROC AUC score = 0.8367

### 2) LightGBM model

- Lgbm Classifier

- GridSearch

- Model Performance 

- Score Table
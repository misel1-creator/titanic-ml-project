# Titanic Survival Prediction

## Project Overview
This project uses machine learning to predict whether a passenger survived the Titanic disaster.

## Problem Type
Classification

## Dataset
Source: Kaggle Titanic Dataset

Files used:
- `train.csv`
- `test.csv`

Target variable:
- `Survived`  
  - `0 = No`
  - `1 = Yes`

## Dataset Overview
- Training Data Shape: 891 rows, 12 columns
- Test Data Shape: 418 rows, 11 columns

## Data Preprocessing
The following preprocessing steps were applied:
- Filled missing values in `Age` using the mean
- Filled missing values in `Embarked` using the mode
- Filled missing values in `Fare` in the test set using the mean
- Encoded `Sex` using LabelEncoder
- Applied one-hot encoding to `Embarked`
- Created a new feature called `FamilySize` using `SibSp + Parch`
- Dropped unnecessary columns:
  - `PassengerId`
  - `Name`
  - `Ticket`
  - `Cabin`

## Exploratory Data Analysis
Key findings:
- Female passengers had a higher survival rate
- First-class passengers had a higher survival rate
- Passenger class and gender were important factors for survival

## Models Used
This project uses 3 machine learning algorithms:
1. Logistic Regression
2. Decision Tree
3. Random Forest

## Hyperparameter Tuning
Random Forest was improved using `GridSearchCV`.

Best parameters:
- `max_depth = 4`
- `n_estimators = 100`

## Evaluation Metrics
The models were compared using:
- Accuracy
- Precision
- Recall
- F1-score

A confusion matrix was also used for the best model.

## Best Model
The best-performing model was **Tuned Random Forest**.

## Output Files
This project generates:
- `submission.csv`
- `titanic_data_dictionary.csv`

## How to Run
1. Make sure the following files are in the project folder:
   - `train.csv`
   - `test.csv`
   - `titanic.ipynb`

2. Install required libraries:
```bash
pip install pandas numpy matplotlib scikit-learn notebook

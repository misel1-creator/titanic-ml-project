# 🚢 Titanic Survival Prediction

## 📌 Project Overview
This project uses machine learning to predict whether a passenger survived the Titanic disaster.

---

## 📊 Dataset
Kaggle Titanic dataset containing passenger features:
- Age, Gender, Class, Fare, Family size

Target:
- Survived (0 = No, 1 = Yes)

---

## 🔍 EDA Insights
- Females had higher survival rates
- First-class passengers survived more
- Higher fare increased survival chances

---

## ⚙️ Data Preprocessing
- Filled missing values (Age, Embarked, Fare)
- Encoded categorical variables
- Created FamilySize feature
- Removed irrelevant columns

---

## 🤖 Models Used
- Logistic Regression
- Decision Tree
- Random Forest

---

## 📏 Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score

---

## ⚙️ Hyperparameter Tuning
GridSearchCV was used to optimize Random Forest parameters.

---

## 📈 Results
- Logistic Regression: ~78%
- Decision Tree: ~80%
- Random Forest: ~85%

Random Forest performed best.

---

## 📊 Visualization
- Survival count chart
- Gender vs survival
- Class vs survival
- Confusion matrix
- Model comparison chart

---

## 🧪 How to Run
pip install -r requirements.txt  
Open titanic.ipynb and Run All

---

## 👥 Contributors
- Ms Orn Soramatey: Logistic Regression
- Ms Em Narong: Decision Tree
- No Missel: Random Forest

---

## 💡 Conclusion
Random Forest achieved the best performance due to its ability to reduce overfitting and handle complex relationships.

---

## 🚀 Future Work
- Add feature engineering (Title extraction)
- Try advanced models (XGBoost)

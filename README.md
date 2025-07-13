# titanic-survival 

Predicting survival on the Titanic using various classification models.

## Dataset

Titanic - Machine Learning from Disaster

https://www.kaggle.com/competitions/titanic

- File used: `train.csv`

## Preprocessing

- Removed irrelevant columns: `PassengerId`, `Name`, `Ticket`, `Cabin`
- Encoded categorical features (`Sex`, `Embarked`)
- Handled missing values in `Age`, `Fare`, and `Embarked`
- Scaled continuous features (`Age`, `Fare`) using StandardScaler

## Models Used

- Logistic Regression  
- Decision Tree  
- Random Forest  
- Gradient Boosting  
- K-Nearest Neighbors  
- Support Vector Machine  
- XGBoost  

## Hyperparameter Tuning

Used GridSearchCV on all models to find the best parameters using 5-fold cross-validation. Accuracy was used as the evaluation metric.

## Evaluation

Metric: Accuracy

| Model               | Accuracy  |
|--------------------|-----------|
| Logistic Regression | 0.7972   |
| Decision Tree       | 0.7203   |
| Random Forest       | 0.8042   |
| Gradient Boosting   | 0.7552   |
| KNN                 | 0.7972   |
| SVM                 | 0.8322   |
| XGBoost             | 0.7902   |


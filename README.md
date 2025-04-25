# Titanic_Survival_Prediction
This is the analysis & prediction of the passengers who were present on the Titanic. It involves Logistic regression for the predictions 

Project Overview
I aim to build a logistic regression model to predict the Survived column using passenger attributes such as:
Age, Sex, Passenger class (Pclass), Fare, Embarkation port (Embarked)

Data Preprocessing
Preprocessing was done using a Pipeline to avoid any data leakage also set best imputation parameters using GridSearchCV  

Numerical Columns(Age, Fare)
Imputation: fill the missing values with the mean of the train & test data
Scaling: Standard Scaler to normanlize the data distribution

Categorical Columns(Sex, Pclass, Embarked)
Imptation: Missing values were filled by the most frequent values(Mode)
Encoding: One-Hot encoding was done 

these(Preprocessing) are done with the ColumnTransformers 

Model Selcetion
as the output is numerical this suggest it is the regression problem also have binary classification hence i have used LogisticRegression 

Model Evaluation 
split the data set in 80/20 train test partitions and do the preprocessing, encoding, imputation using the pipelines and ColumnTransformer  and get the accuracy_score of 1.0 but accuracy be 1 suggest that it is not complete dataset or the combination of sex, embarked and Pclass perfectly determines the survival outcome  which is not usual in real-world data.


Author: 
Made with 💙 by Animesh Porwal(anni0955)
feel free to fork, use, or, contribute

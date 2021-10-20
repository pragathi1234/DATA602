
### Dataset 
https://www.kaggle.com/uciml/pima-indians-diabetes-database. 

### Data Description 
The datasets consists of several medical predictor variables and one target variable, Outcome. Predictor variables includes the number of pregnancies the patient has had, their BMI, insulin level, age, and so on. 

This dataset is classification problem, determining whether or not an individual has diabetes

### Observations 
- Regularization strengths : 0.5,1,2,10,50
- Solvers : liblinear(Works better for smaller datasets), sag
- As this data falls under recall metrics, accuracy got decreased and recall got increased to 61% to 78% after applying GridSearchCV

### Summary 
1. Preprocess data, if any missing values are present
2. Splitted data using train_test_split
3. Created pipeline using logistic regression and standard scalar
4. Picked metrics as recall, accuracy
5. Ran a Logistic Regression model with grid search cross-validation using 10 folds. Search 5 different regularization strengths and 2 solvers. 
6. Though accuracy got decreased by 1%, recall values got increased, so I feel this is good model.

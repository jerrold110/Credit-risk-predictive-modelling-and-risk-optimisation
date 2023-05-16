# Credit risk predictive modelling and risk optimisation

A hypothetical bank has to determine the risk of issuing credit to clients by modelling the probability of loan default and creating a risk model to the business. It then has to optimise profit earned through interest payments from new clients for a certain risk budget which varies from quarter to quarter.

Project is defined and outlined in *Business objective.ipynb*

### Part 1 - EDA
- Analysing relationship between categorical vars and target
- Deciding which categorical variables to convert to numerical, one-hot-encode, embed, and target encoding


### Part 2 - Preprocessing categorical data
- Feature selection with chi2 test for considerations of curse of dimensionality
- One hot encoding
- Encoding categories into target means
- Tokenising text data and converting into vectors and into columns


### Part 3 - Preprocessing numerical data
- Creating selected categorical features into numerical data
- Creating features based on discovered patterns and heuristics


### Part 4 - Feature selection, scaling, oversampling, model selection
- Train test split
- Creating data: unscaled, standardised, normalised 
- Oversampling of minority class
- Cross validated grid search on: 3 types of scaled and unscaled data, optimal features, grid scoring function
- Evaluation of performance metrics: Acc, Recall, Area under ROC
- Models tested: Logistic Reg, Random For, SGD, Gradient Boost, Adaboost(decision Tree), Adaboost(Log Reg), Gaussian process, SVM, XGBoost

### Part 5 - Performance tuning of best models
- Preparation of data (train data in split had to be increased slightly because of underfitting)
- Determining optimal number of features to use with analysis of AUC and number of features
- Tuning parameters with best selected data/model/grid scoring function
- Tuning positive threshold for higher accuracy
- Confusion matrix and ROC curves
- Saving of predicted probability results on test data for next part

### Part 6 - Optimisation of risk budget
- Calculation of interest rate and interest to be paid
- Calculation of risk factor with Probability of default and credit amount based on risk model
- Determining maximum POD threshold to offer credit based on ideal POD threshold for positive class (det. in part V)
- Optimising for max profit as given risk budget by determining which clients to offer/reject with Mixed-integer linear programming
- Visualising POD and interest rates/amounts of approved credit to understand risk portfolio (presentation to management)
- Conclusion


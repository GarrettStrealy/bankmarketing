In this project I implemented machine learning algorithms in Python to accurately predict the results of a bank's marketing campaign. This project demonstrates my ablity to utilize various libraries in Python to perform applied machine learning with high accuracy.

### Analysis

#### Algorithms ranked by performance:

Random Forest: 100% accuracy

Naive Bayes: 98%

Logistic Regression: 90%

kNN: 89%

Random Forest and Naive Bayes achieved very similar accuracy. Naive Bayes was worse in precision for target 0 (91% vs 100% for Random Forest).

### The two tree models may have outperformed Linear Regression for the following reasons:

#### Linear separability: 
The data may not be linearly separable. Logistic Regression assumes that the data is linearly (or curvy linearly) separable in space. Trees are non-linear classifiers; they do not require data to be linearly separable.

#### Skewness: 
The predictors displacement, horsepower, and weight are moderately/highly skewed. Trees handle skewed predictors nicely if allowed to grow fully. Logistic Regression does not handle skewed predictors well.

#### Outliers: 
There may be some unhandled outliers influencing the Logistic Regression. Logistic Regression will push the decision boundary towards an outlier. Trees, at the initial stage, won't be affected by an outlier. However, if we let them grow fully, the signal will mote to one side (+ve or -ve), while the outlier will be moved to the other (there will be one leaf for each outlier).

Even with proper scaling provided for fair treatment among features, kNN performed worst of the four.

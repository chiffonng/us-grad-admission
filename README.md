
# US Masters Admission: A Regression Analysis

This repository contains a regression analysis to predict the chance of admission to US Masters programs for international students, from an Indian perspective. The model, built using the statsmodel library, shows that undergraduate GPA is the strongest predictor for chance of graduate admission, with a correlation of 0.88.

### Regression Analysis 
The model is a linear regression model that predicts the chance of admission based on the input features. It found a strong positive correlation of 0.88 between GPA and Chance of Admission in the sample. Correlation coefficient significance test and confidence interval validates there's evidence for a linear relationship between them in the population of international applicants to US Masters program.

The [notebook](https://github.com/chiffonng/us-grad-admission/blob/main/US%20Graduate%20Admission%20Prediction.ipynb) also includes validity checks for LINH assumptions before conducting regression analysis:
- **Linearity**: There exists a linear relationship between two quantitative variables, tested with a *scatterplot* `sns.pairplot`
- **Independence of observations**: Each observation in the dataset is independent.
- **Normality of errors**: The plot of errors is relatively normally distributed `statsmodels.api.qqplot`
- **Homoscedasticity of residuals**: The residuals have **constant variance** at every level of the independent variable. It could be checked by creating a _fitted value vs. residual plot_ 
- **Little to no multicollinearity** (for multiple regression): No or little correlation between pairs of independent variables. 
### Dataset

The dataset used for this model is the [Graduate Admissions dataset](https://www.kaggle.com/mohansacharya/graduate-admissions) from Kaggle. It contains information about the GRE scores, TOEFL scores, university rating, statement of purpose, letter of recommendation, and GPA of students applying to US graduate schools.

### Acknowledgments
Graduate Admissions dataset from [Kaggle](https://www.kaggle.com/datasets/mohansacharya/graduate-admissions)

**Name: Kartik Tyagi**\
**Reg No: 23BAI10360**\
**Application no: IN26010566**\
**Batch Number: 1(A)**

# AI-ML-Assignment-3
Salary Prediction using Polynomial Regression
# Position Salaries - Polynomial Regression

## Objective
The objective of this project is to develop a Polynomial Regression model to estimate the salary of employees based on their position level. Since the relationship between position level and salary is non-linear, a polynomial approach is used to accurately predict compensation.

## Dataset Link
[Position Salaries Dataset on Kaggle](https://www.kaggle.com/datasets/akram24/position-salaries)

## Libraries Used
* **Pandas**: For data loading, manipulation, and analysis.
* **NumPy**: For numerical operations and generating grid values for smooth plotting.
* **Scikit-Learn (sklearn)**: For model building (`LinearRegression`, `PolynomialFeatures`), data splitting (`train_test_split`), and evaluation metrics.
* **Matplotlib**: For visualizing the original data points and the polynomial regression curve.

## Methodology
1. **Data Understanding**: Loaded the dataset to identify the input feature (`Level`) and target variable (`Salary`).
2. **Data Preprocessing**: Checked for missing values and split the dataset into training (80%) and testing (20%) sets.
3. **Model Development**: Transformed the input feature into polynomial features (Degree = 3) using `PolynomialFeatures` and trained a `LinearRegression` model on this transformed data.
4. **Model Evaluation**: Assessed the model's performance using Mean Absolute Error (MAE), Mean Squared Error (MSE), and $R^2$ Score. Visualized the fit using a scatter plot overlaid with the polynomial curve.

## Results
The Polynomial Regression model (Degree = 3) fits the dataset significantly better than a standard linear model. 
* The curve accurately tracks the relatively flat trajectory of lower-level salaries and perfectly captures the steep, exponential-like increase for executive positions (Levels 8-10). 
* Evaluation metrics confirm that the polynomial model explains a high amount of the variance in the target variable, making it highly accurate for interpolation within the 1-10 level range.

## Conclusion
The project successfully demonstrates the necessity of Polynomial Regression for non-linear datasets. Standard Linear Regression would heavily underfit this data, resulting in large prediction errors for higher levels. By adding polynomial terms, the regression line bends to capture the true exponential nature of corporate compensation structures. This flexibility makes Polynomial Regression an ideal and effective choice for predicting these position salaries.

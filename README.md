 Used Car Price Prediction
Predicting the price of used cars with a linear regression model using Python and popular data science libraries.



##Project Overview
This project aims to build a linear regression model to predict used car prices by leveraging various data preprocessing and feature engineering techniques. The model follows standard Ordinary Least Squares (OLS) assumptions and applies feature transformations to enhance prediction accuracy.

Tools and Libraries Used
Python
Pandas: For data loading, cleaning, and manipulation
NumPy: For numerical operations
scikit-learn: For model training, testing, and evaluation
statsmodels: For statistical tests and regression analysis
Matplotlib and Seaborn: For data visualization
Project Workflow
1. Loading the Data
The dataset is loaded from a CSV file in the project directory using Pandas.

2. Preprocessing
Handling Missing Values
We check for missing values and impute or remove them as appropriate.

Removing Unnecessary Columns
The Model column was deemed unnecessary for our regression and was excluded from the final feature set.

3. Exploratory Data Analysis (EDA)
Exploring Distributions (PDFs)
We plot distributions for the variables to understand their spread and to spot any anomalies, like outliers.

Outlier Detection and Treatment
Outliers in the data can affect the OLS regression, so they are addressed by either capping, transforming, or removing.

4. Checking OLS Assumptions
To improve the model's performance and validity, we check assumptions for OLS regression, including linearity, normality of residuals, homoscedasticity, and absence of multicollinearity.

Transforming Variables
A log transformation is applied to Price to meet the assumption of normality.

Multicollinearity Check
Variance Inflation Factor (VIF) is used to check for multicollinearity among predictors. The Year variable, with the highest VIF, is removed to reduce multicollinearity.

5. Data Scaling and Train-Test Split
The data is scaled for better regression performance, and an 80-20 train-test split is applied with a set random state for reproducibility.

6. Building the Linear Regression Model
A linear regression model is trained and tested on the preprocessed data.

7. Model Evaluation
The model is evaluated using metrics like Mean Squared Error (MSE) and R-squared.

Results and Insights
The model successfully predicts used car prices with reasonable accuracy after handling missing data, treating outliers, and addressing multicollinearity. Data visualization and variable transformations improved the model’s performance.

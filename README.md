# Used Car Price Prediction

## Project Overview
This project aims to build a **linear regression model** to predict used car prices using various data preprocessing and feature engineering techniques. The model follows the standard **Ordinary Least Squares (OLS)** assumptions and applies feature transformations to enhance prediction accuracy.

## Tools and Libraries Used
- **Python**
- **Pandas**: For data loading, cleaning, and manipulation
- **NumPy**: For numerical operations
- **scikit-learn**: For model training, testing, and evaluation
- **statsmodels**: For statistical tests and regression analysis
- **Matplotlib** and **Seaborn**: For data visualization

## Project Workflow

### 1. Loading the Data
- The dataset is loaded from a CSV file in the project directory using **Pandas**.

### 2. Preprocessing
#### Handling Missing Values
- We check for missing values and handle them by imputing or removing them, depending on the nature of the data.

#### Removing Unnecessary Columns
- The **Model** column was deemed unnecessary for our regression and was excluded from the final feature set.

### 3. Exploratory Data Analysis (EDA)
#### Exploring Distributions (PDFs)
- We plot distributions for the variables to understand their spread and to identify anomalies like **outliers**.

#### Outlier Detection and Treatment
- Outliers in the data can affect the **OLS regression**, so they are addressed by either **capping**, **transforming**, or **removing**.

### 4. Checking OLS Assumptions
To ensure the regression model’s validity and performance, we check the following **OLS assumptions**:
- **Linearity** of the relationships between predictors and target
- **Normality of residuals**
- **Homoscedasticity** (constant variance of errors)
- Absence of **multicollinearity**

#### Transforming Variables
- A **log transformation** is applied to the **Price** to meet the assumption of normality.

#### Multicollinearity Check
- The **Variance Inflation Factor (VIF)** is used to check for multicollinearity. The **Year** variable, with the highest VIF, is removed to reduce multicollinearity.

### 5. Data Scaling and Train-Test Split
- The data is **scaled** to improve regression performance, and an **80-20 train-test split** is applied with a set **random state** for reproducibility.

### 6. Building the Linear Regression Model
- A **linear regression model** is trained and tested on the preprocessed data.

### 7. Model Evaluation
- The model is evaluated using metrics like:
  - **Mean Squared Error (MSE)**
  - **R-squared (R²)**

## Results and Insights
The model successfully predicts **used car prices** with reasonable accuracy. After handling missing data, treating outliers, and addressing multicollinearity, the model's performance improved significantly. Additionally, **data visualization** and **variable transformations** played a key role in enhancing the model's overall performance.

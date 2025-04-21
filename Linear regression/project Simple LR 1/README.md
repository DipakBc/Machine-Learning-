# Medical Insurance Cost Prediction using Linear Regression-Simple Linear Regression

## Problem Statement

The goal of this project is to develop a machine learning model that predicts the medical insurance cost of individuals based on several features such as age, sex, BMI, number of children, smoking habits, and residential region. Predicting insurance costs accurately can help insurance companies estimate potential expenses and optimize pricing strategies.

## Dataset

The dataset used for this project is `insurance.csv`, which contains the following columns:

- `age`: Age of the individual
- `sex`: Gender of the individual
- `bmi`: Body Mass Index
- `children`: Number of children covered by health insurance
- `smoker`: Whether the person smokes or not
- `region`: Residential region of the individual in the US
- `charges`: Medical insurance cost (target variable)

## Approach

1. **Data Loading and Exploration**: Loaded the dataset using pandas and explored its structure and descriptive statistics.
2. **Data Visualization**: Used pair plots and heatmaps to visualize relationships and correlations between features.
3. **Preprocessing**:
   - Applied OneHotEncoding to categorical variables (`sex`, `smoker`, `region`).
   - Scaled numerical features (`age`, `bmi`, `children`) using StandardScaler.
4. **Model Building**:
   - Created a pipeline using `ColumnTransformer` and `Pipeline` from scikit-learn.
   - Used `LinearRegression` as the prediction model.
5. **Training and Evaluation**:
   - Split the dataset into training and testing sets.
   - Trained the model and evaluated it using R-squared and Mean Squared Error (MSE).
6. **Visualization**:
   - Plotted actual vs. predicted values.
   - Visualized the impact of each feature using coefficient bar charts.
7. **Prediction**:
   - Made predictions on new, unseen data.
   - Compared the prediction against the distribution of actual charges.

## Evaluation

- **R² Score**: 0.7347
- **Mean Squared Error**: 38,291,133.01

These metrics indicate a decent model performance, capturing around 73% of the variance in insurance charges.

## Future Improvements

- Try other regression models such as Ridge, Lasso, or Random Forest for better accuracy.
- Perform feature selection or dimensionality reduction.
- Handle outliers in BMI or charges to improve model robustness.

## Author

Dipak Budha Chhetri

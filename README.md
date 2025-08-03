# CODEALPHA_4

## TASK 4: Sales Prediction using Python

This project predicts product sales based on advertising spend in TV, Radio and Newspaper channels using various regression models.

##  Models Used
- Linear Regression
- Ridge & Lasso Regression
- Decision Tree Regressor
- Random Forest Regressor
- XGBoost Regressor

## Evaluation Metrics
- Mean Squared Error (MSE)
- R² Score

## Libraries Used
- pandas, matplotlib, seaborn
- scikit-learn
- xgboost
- plotly (for visualization)

## **Dataset Features:**

| Feature      | Description                             |
| ------------ | --------------------------------------- |
| `TV`         | Advertising spend on TV (in thousands)  |
| `Radio`      | Advertising spend on Radio              |
| `Newspaper`  | Advertising spend on Newspaper          |
| `Sales`      | Sales generated (in thousands of units) |
| `Unnamed: 0` | Index column (not used)                 |

## **Steps Followed:**

#### 1. **Data Loading and Preprocessing**

* Checked for missing values —  None found.
* Dropped the `Unnamed: 0` index column.
* Verified datatypes and basic statistics.

#### 2. **Exploratory Data Analysis (EDA)**

* Scatter plots:

  * **TV vs Sales**: Strong positive correlation.
  * **Radio vs Sales**: Moderate positive correlation.
  * **Newspaper vs Sales**: Weak/No correlation.
* Outlier detection: No significant outliers observed.

#### 3. **Time Series Visualization**

* Created a **date range** and visualized `Sales` over time using **Plotly**.
* Observed high fluctuations, spikes around mid-June.
* No clear trend or seasonality identified visually.

#### 4. **Regression Models Applied**

| Model                   | R² Score |
| ----------------------- | -------- |
| Linear Regression       | 0.899   |
| Ridge Regression        | 0.899   |
| Lasso Regression        | 0.899   |
| Decision Tree Regressor | 0.931   |
| Random Forest Regressor | 0.981   |
| XGBoost Regressor       | 0.972   |

## **Conclusion:**

* Advertising spend, especially on **TV and Radio**, plays a crucial role in boosting sales.
* **Newspaper ads** offer diminishing returns.
* Businesses should consider **allocating more budget to TV and Radio**.
* Tree-based regressors (Random Forest, XGBoost) are excellent choices for accurate sales forecasting.
* Time-based sales forecasting can be enhanced using **ARIMA/Prophet** for deeper trend analysis.






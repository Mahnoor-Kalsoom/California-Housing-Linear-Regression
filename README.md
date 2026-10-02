# California Housing Price Prediction using Linear Regression

This project is a beginner-friendly implementation of **Linear Regression** using the **California Housing dataset** from Scikit-learn.

The main goal of this project is to understand the basic end-to-end workflow of a **Supervised Machine Learning regression problem**. The project focuses on using **Median Income (`MedInc`)** to predict **Median House Value (`MedHouseVal`)**.

The project covers data loading, data exploration, feature selection, visualization, model training, prediction, evaluation, and making predictions on new input values.

---

## Machine Learning Approach

* **Learning Type:** Supervised Learning
* **Problem Type:** Regression
* **Algorithm:** Linear Regression
* **Input Feature:** Median Income (`MedInc`)
* **Target Variable:** Median House Value (`MedHouseVal`)

Since only one input feature is used, this project demonstrates **Simple Linear Regression**.

---

## Dataset

The project uses the **California Housing dataset**, which is available through Scikit-learn.

The complete dataset contains:

* **20,640 samples**
* **8 input features**
* **1 target variable**

For this project, only the **Median Income (`MedInc`)** feature is selected as the input. Using a single feature makes it easier to understand the basic relationship between an input variable and the target variable.

### Selected Variables

| Variable      | Description                              |
| ------------- | ---------------------------------------- |
| `MedInc`      | Median income of households in the block |
| `MedHouseVal` | Median house value in the block          |

---

## Project Workflow

The project follows these steps:

1. Load the California Housing dataset
2. Explore the dataset
3. Convert the dataset into a Pandas DataFrame
4. Save the dataset as a CSV file
5. Check the dataset columns and missing values
6. Select `MedInc` as the input feature
7. Select `MedHouseVal` as the target variable
8. Visualize the relationship between median income and house value
9. Split the data into training and testing sets
10. Train a Linear Regression model
11. Generate predictions on the test data
12. Compare actual and predicted values
13. Visualize the regression results
14. Evaluate the model using MAE, MSE, and R² Score
15. Make predictions using new input values

---

## Technologies and Libraries

* **Python**
* **Google Colab**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Scikit-learn**

---

## Model Training

The Linear Regression model is created using Scikit-learn:

```python
from sklearn.linear_model import LinearRegression

model = LinearRegression()

model.fit(X_train, y_train)
```

After training, the model is used to predict house values from the test data:

```python
y_pred = model.predict(X_test)
```

---

## Model Evaluation

The model performance is evaluated using three common regression metrics:

### Mean Absolute Error (MAE)

MAE measures the average absolute difference between the actual and predicted values.

### Mean Squared Error (MSE)

MSE measures the average squared difference between the actual and predicted values. Larger errors have a greater effect on this metric.

### R² Score

R² Score measures how much of the variation in the target variable can be explained by the model.

These metrics help evaluate how well the Linear Regression model predicts median house values from median income.

---

## Visualization

The project includes visualizations to better understand the relationship between the input feature and the target variable.

The visualizations include:

* Relationship between **Median Income** and **Median House Value**
* Linear Regression line
* Actual vs. predicted values

These plots provide a visual understanding of how the trained model fits the data.

---

## Example Prediction

After training the model, it can also be used to predict house values for new median-income values.

For example:

```python
new_income = [[5.0]]

predicted_value = model.predict(new_income)

print(predicted_value)
```

This demonstrates how a trained Machine Learning model can be used to make predictions on new data.

---

## Learning Outcomes

Through this project, I practiced the basic workflow of a supervised Machine Learning regression problem, including:

* Understanding features and target variables
* Loading and exploring a dataset
* Data preparation using Pandas
* Selecting relevant features
* Splitting data into training and testing sets
* Training a Linear Regression model
* Generating predictions
* Evaluating regression models
* Using MAE, MSE, and R² Score
* Visualizing data and model predictions
* Making predictions using new input data

---

## Future Improvements

The current project uses only **Median Income (`MedInc`)** as the input feature to demonstrate Simple Linear Regression.

A future version can use all available housing features to implement **Multiple Linear Regression**.

Possible improvements include:

* Using all 8 input features
* Comparing Simple Linear Regression with Multiple Linear Regression
* Comparing different Machine Learning algorithms
* Performing feature analysis
* Improving model performance through feature engineering
* Using additional evaluation and visualization techniques

---

## Project Files

```text
California-Housing-Linear-Regression/
│
├── california_housing_linear_regression.ipynb
├── california_housing.csv
└── README.md
```

### `california_housing_linear_regression.ipynb`

Contains the complete Python implementation, including data exploration, visualization, model training, predictions, and evaluation.

### `california_housing.csv`

Contains the California Housing dataset used in the project.

### `README.md`

Provides an overview of the project, methodology, workflow, technologies, and learning outcomes.

---

## Author

**Mahnoor Kalsoom**

Machine Learning Practice Project

GitHub: [Mahnoor-Kalsoom](https://github.com/Mahnoor-Kalsoom)

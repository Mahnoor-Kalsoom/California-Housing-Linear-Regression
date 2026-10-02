\# California Housing Price Prediction using Linear Regression



This project is a beginner-friendly implementation of \*\*Linear Regression\*\* using the California Housing dataset.



The goal of the project is to understand the complete basic Machine Learning workflow, including loading a real-world dataset, exploring the data, selecting features, splitting data into training and testing sets, training a model, making predictions, evaluating performance, and visualizing the results.



\## Machine Learning Approach



\- \*\*Learning Type:\*\* Supervised Learning

\- \*\*Problem Type:\*\* Regression

\- \*\*Algorithm:\*\* Linear Regression

\- \*\*Input Feature:\*\* Median Income (`MedInc`)

\- \*\*Target:\*\* Median House Value (`MedHouseVal`)



\## Dataset



The project uses the California Housing dataset available through Scikit-learn.



The complete dataset contains:



\- 20,640 samples

\- 8 input features

\- 1 target variable



For this beginner implementation, only `MedInc` is used as the input feature so that the basic concept of Simple Linear Regression can be clearly understood.



\## Project Workflow



1\. Load the California Housing dataset

2\. Explore the dataset

3\. Save the dataset as CSV

4\. Check columns and missing values

5\. Select input feature and target

6\. Visualize the relationship between income and house value

7\. Split the dataset into training and testing sets

8\. Train a Linear Regression model

9\. Generate predictions

10\. Compare actual and predicted values

11\. Visualize the regression results

12\. Evaluate the model using MAE, MSE, and R²

13\. Make predictions using new input values



\## Technologies Used



\- Python

\- Google Colab

\- Pandas

\- NumPy

\- Matplotlib

\- Scikit-learn



\## Model Training



The model is trained using:



```python

model = LinearRegression()

model.fit(X\_train, y\_train)



Predictions are generated using:

y\_pred = model.predict(X\_test)





Model Evaluation

The model is evaluated using:

\- Mean Absolute Error (MAE)

\- Mean Squared Error (MSE)

\- R² Score

These metrics help measure how closely the predicted house values match the actual values.

Learning Outcome

This project demonstrates the basic end-to-end workflow of a supervised Machine Learning regression problem.

It provides practical experience with:

\- Features and targets

\- Training and testing data

\- Linear Regression

\- Model fitting

\- Predictions

\- Regression evaluation metrics

\- Data visualization

Future Improvements

The next version of the project can use all available housing features instead of only median income. This will demonstrate Multiple Linear Regression and allow comparison with the single-feature model.

Author

Mahnoor Kalsoom

Machine Learning Practice Project


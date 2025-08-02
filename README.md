# Linear Regression for Real Estate Price Prediction
This project demonstrates how to perform linear regression using Python's `scikit-learn` library to predict real estate prices based on a given dataset.

## Description
The Python script reads a CSV file named `Real_estate.csv`, which contains data about different properties. It then builds a linear regression model to predict the `Price` of a property based on several of its features.

The features used for prediction are:
* `Has_Garden`
* `Num_Bedrooms`
* `Num_Floors`
* `Square_Feet`
* `Year_Built`

The script will train the model, evaluate its performance, and generate a plot to visualize the relationship between the actual and predicted prices.

## Prerequisites
Before running the script, you need to have Python installed, along with the following libraries:

* `pandas`
* `scikit-learn`
* `matplotlib`

You can install these libraries using `pip`:
```python
pip install pandas scikit-learn matplotlib
```

## How to Run
Make sure you have the `Real_estate.csv` file in the same directory as the Python script.

Run the script from your terminal:
```
python linear_regression.py
```

## Output
The script will produce the following output:

1. **Model Details in the Console**:
* *Coefficients*: These numbers show the impact of each feature on the house price. For example, a positive coefficient for `Num_Bedrooms` means that, on average, the price increases as the number of bedrooms increases.
* *Intercept*: This is the theoretical base price of a house if all other features were zero.
* *Mean Squared Error (MSE)*: This measures the average squared difference between the actual and predicted prices. A lower MSE indicates a better fit.
* *R-squared*: This value, between 0 and 1, indicates how much of the variation in house prices can be explained by our model. For example, an R-squared of 0.85 means that 85% of the price variations can be explained by our model's features.

2. **A Plot**:
A scatter plot named `actual_vs_predicted.png` will be saved in the same directory. This plot helps you visualize the model's performance by showing how close the predicted prices (on the y-axis) are to the actual prices (on the x-axis). The more the points align in a straight diagonal line, the better the model's predictions.

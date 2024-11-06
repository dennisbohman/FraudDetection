# Card Fraud Detection – How the Code Works

This project is a step-by-step guide for building a model to predict fraudulent credit card transactions. Here’s a breakdown of what each part of the code does:

## 1. Load the Dataset and Explore the Data

First, we load the dataset and do a quick analysis to understand its structure:

- **Load the data**: The dataset is loaded with `pandas`, so we can start working with it right away.
- **Basic EDA** (Exploratory Data Analysis): We print out data types and some basic stats to get a feel for what we’re working with.
- **Check for fraud cases**: We quickly look at how many transactions are labeled as fraudulent versus legitimate.

## 2. Feature Engineering – Create New Variables

To improve the model’s performance, we create a new variable:

- **Distance variable**: We calculate the difference between the distance from home and the distance of the last transaction. The idea is that large changes in distance might signal fraud.

## 3. Visualization

Time to visualize the data and see if we can spot any interesting patterns:

- **Correlation matrix**: We draw a heatmap to see correlations between different variables. This can help us spot relationships that might be useful for the model.
- **Scatterplot with linear regression**: We use a scatterplot to look at the relationship between distance from home and the ratio to the median purchase amount.

## 4. Split the Data into Training and Test Sets

To properly evaluate the model, we split the data:

- **Training and test data**: We split the data so we can train on one part and evaluate on another, which helps us see how well the model generalizes.

## 5. Train and Evaluate the Model

Now we get to the machine learning part:

- **Train the model**: We use a simple logistic regression to do the classification.
- **Make predictions**: With the trained model, we predict if the transactions in the test set are fraudulent or not.
- **Evaluate**: Finally, we print out the model’s accuracy to get an idea of how well it does at identifying fraud.

---

And that’s it! The code is straightforward to follow and creates a basic model for spotting fraud in credit card transactions.

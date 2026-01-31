# python-ml-project
A simple machine learning project using Linear Regression to predict student exam scores based on study hours.
# Student Score Prediction — Linear Regression

This project is a simple machine learning model that predicts **student exam scores** based on the number of **hours studied**.  
It uses a **Linear Regression** model from scikit-learn and is designed as a beginner-friendly ML project.

---

## Tools & Libraries Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  
- Google Colab  

---

##  What This Project Does
- Loads a dataset of **study hours vs exam scores**
- Visualizes how study time impacts performance
- Splits the data into **training** and **testing**
- Trains a **Linear Regression** model
- Makes predictions
- Visualizes the regression line
- Saves predictions to a CSV file

---

## Project Structure
python-ml-project/
│── ml_model.ipynb # Complete Google Colab notebook
│── hours.csv # Dataset used for training
│── predictions.csv # Model predictions on test data
│── README.md # Project documentation




---

## Model Workflow
1. Import dataset (`hours.csv`)  
2. Scatter plot of hours vs scores  
3. Train/test split  
4. Train Linear Regression model  
5. Predict exam scores  
6. Compare actual vs predicted  
7. Plot regression line  
8. Export predictions to `predictions.csv`  

---

## Example Output
A student who studies **5 hours** is predicted to score around **50–55 marks**, based on the regression model.

---

## How to Run

Install necessary libraries:

```bash
pip install pandas numpy matplotlib scikit-learn


import pandas as pd
from sklearn.linear_model import LinearRegression

df = pd.read_csv("hours.csv")
model = LinearRegression()
model.fit(df[["Hours"]], df["Scores"])
```
## Dataset

The dataset contains two columns:

| Hours | Scores |
|-------|--------|
| 2.5   | 21     |
| 5.1   | 47     |
| 3.2   | 27     |
| ...   | ...    |

## Purpose

This project demonstrates a complete beginner-friendly machine learning workflow:
- data loading
- visualization
- model training
- prediction
- evaluation
- exporting results


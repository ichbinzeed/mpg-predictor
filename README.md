# 🚗 MPG Prediction for Cars from Japan, USA, and Europe

![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn%2C%20Pandas%2C%20Numpy-brightgreen.svg)

## 📋 Project Overview

This project focuses on predicting the **miles per gallon (MPG)** of cars from different regions (Japan, USA, and Europe) based on several key features. The dataset includes cars from different time periods and origins, and the prediction is based on their characteristics, such as:

- Cylinders
- Displacement
- Horsepower
- Weight
- Acceleration
- Model Year
- Origin (Region of the car: Japan, USA, Europe)

I experimented with several machine learning models, including Linear Regression, Ridge, and Lasso Regression. After extensive experimentation, **Lasso Regression** with polynomial features was selected as the optimal model for this task, after tuning the hyperparameters using **RandomizedSearchCV**.

## 📈 Best Model

After trying different models, the best performing model was **Lasso Regression**. The hyperparameters were optimized using **RandomizedSearchCV**, leading to the following configuration:

- **Best Parameters**: 
  - `regression__fit_intercept`: `False`
  - `regression__alpha`: `0.1`
  - `poly__degree`: `3` (Degree of the polynomial features)

### Performance Metrics

- **Mean Squared Error (MSE)**: `5.8604848427844916`
- **Root Mean Squared Error (RMSE)**: `2.4208438286648093`
- **Standard Deviation of Error**: `7.67723221134341`

These metrics show that the model performs well in predicting the MPG for cars based on the given features.

## 📊 Features Used for Prediction

The prediction model was built using the following features from the dataset:

- `Cylinders`: Number of cylinders in the engine
- `Displacement`: Engine displacement (size)
- `Horsepower`: Engine power
- `Weight`: Weight of the car
- `Acceleration`: Time taken to accelerate from 0 to a certain speed
- `Model Year`: Year the car was produced
- `Origin`: Origin of the car (Japan, USA, or Europe)

## 🔧 Tools and Libraries

- **Python**: Version 3.8+
- **Scikit-learn**: For model building and evaluation
- **Pandas**: For data manipulation
- **Numpy**: For numerical computations
- **RandomizedSearchCV**: For hyperparameter tuning

## 🎯 Educational Purpose

This project is **educational** and part of my learning journey in machine learning. I'm currently experimenting with different models and techniques to improve my understanding of data science and model optimization. 

While the results presented here are based on my experiments, there is still room for improvement and learning. Contributions and feedback are always welcome as I continue developing my skills in this area.

## 🤝 Contributing

Feel free to submit pull requests or open issues if you have any suggestions or improvements!

---

### 🏎️ Happy Predicting!


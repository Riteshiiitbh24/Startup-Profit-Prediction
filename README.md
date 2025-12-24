📈 Startup Profit Prediction using Linear & Regularized Regression
📌 Overview

This project implements an end-to-end Startup Profit Prediction system using Linear Regression and Regularized Regression (Ridge).
The focus is on understanding model behavior, overfitting, regularization, and the bias–variance tradeoff, while also extracting actionable business insights.

🎯 Problem Statement

Given startup-related features such as:

R&D Spend

Administration Cost

Marketing Spend

State (categorical)

Predict the Profit of a startup and analyze how different expenses impact profitability.

📂 Dataset

Dataset: 50 Startups Dataset

Target Variable: Profit

Features: R&D Spend, Administration, Marketing Spend, State

🛠️ Tech Stack

Python

NumPy

Pandas

Matplotlib

Scikit-learn

🔄 Project Workflow
1️⃣ Data Preprocessing

One-hot encoding for categorical features

Feature scaling using StandardScaler

Train–test split

2️⃣ Baseline Linear Regression (From Scratch)

Implemented Linear Regression using Batch Gradient Descent

Manually computed gradients and updated weights

Tracked training loss across iterations

Evaluation:

Train & Test Mean Squared Error (MSE)

Loss vs Iterations

Actual vs Predicted Profit

✅ Result: Baseline model shows good generalization (train ≈ test error).

3️⃣ Overfitting Demonstration

Introduced Polynomial Features (degree = 3)

Trained the same linear regression model

❌ Result:

Training error decreases significantly

Test error increases sharply
➡️ Clear overfitting

4️⃣ Ridge Regression (Regularization)

Implemented Ridge Regression (from scratch and using sklearn)

Penalized large coefficients to control variance

✅ Result:

Slight increase in training error

Significant reduction in test error
➡️ Overfitting successfully fixed

5️⃣ Bias–Variance Tradeoff Analysis

Trained Ridge models with multiple alpha (λ) values

Plotted Alpha vs Train/Test Error

📉 Insight:

Low α → Overfitting

High α → Underfitting

Optimal α minimizes test error

📊 Visualizations

Loss vs Iterations (Gradient Descent Convergence)

Actual vs Predicted Profit

Overfitting comparison

Alpha vs Error (Bias–Variance Tradeoff)

💼 Business Insights

R&D Spend is the strongest driver of startup profit

Marketing Spend has diminishing returns

Administrative Cost has minimal direct impact

Regularized models provide more reliable financial predictions

✅ Key Takeaways

Built regression models from scratch to understand core ML mechanics

Demonstrated and fixed overfitting using Ridge regularization

Visualized bias–variance tradeoff for hyperparameter tuning

Combined technical modeling with business decision insights




# linear-regression-from-scratch-student-performance
This project implements Linear Regression from scratch using Python to predict students' final grades (G3) based on their earlier exam scores (G1 and G2). The goal is to understand the fundamentals of machine learning algorithms by implementing them manually instead of using pre-built libraries.

Dataset

Source: Student Performance Dataset (UC Irvine ML Repository).


Description: Academic records from two Portuguese secondary schools covering demographics, social attributes, and grades.


Key Variables: * G1: First period grade (Feature).


G2: Second period grade (Feature).


G3: Final grade (Target Variable).

Methodology
1. Linear Regression Model
The model uses the following hypothesis function:
y = (w1 * x1) + (w2 * x2) + b


x1, x2: Input features (G1 and G2).

w1, w2: Model weights.

b: Bias term.

2. Loss Function
The objective is to minimize the Mean Squared Error (MSE):
MSE = (1/n) * Σ (y_true - y_pred)^2
Gradient Descent is used to iteratively update the weights and bias.

3. Training Process
Initialize weights and bias.

Compute predictions and calculate MSE loss.

Compute gradients and update parameters.

Repeat until the loss curve converges.

Model Evaluation
Performance is measured using Root Mean Squared Error (RMSE) on both training and test sets:
RMSE = sqrt(MSE)

Bonus Task: Predicting G3 without G1 and G2
In this experiment, G1 and G2 were excluded to predict G3 using only demographic and social attributes.


Observation: Prediction becomes significantly harder as other features have a weaker correlation with the final grade compared to prior academic performance.


Result: This led to a higher RMSE and demonstrated the critical importance of feature selection.

Technologies Used
Python: Core programming language.

NumPy / Pandas: Data manipulation and matrix operations.

Matplotlib: Plotting the MSE loss curve and results.

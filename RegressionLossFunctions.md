# 📉 Common Regression Loss Functions

These loss functions measure the difference between predicted and actual values in machine learning regression tasks. Here’s a breakdown:

---

## 1. Max Absolute Error (MaxAE)

**Definition:**  
Measures the largest absolute error between predicted and actual values.

**Formula:**  
MaxAE = max( | y_true - y_pred | )

**Focus:**  
Only the worst-case scenario (largest mistake).

**Use case:**  
When you care about the single worst error, such as ensuring no extreme failures in engineering models.

---

## 2. Mean Absolute Error (MAE)

**Definition:**  
Measures the average absolute difference between predicted and actual values.

**Formula:**  
MAE = (1/n) * Σ | y_true - y_pred |

**Focus:**  
Gives a more balanced view of errors without squaring them.

**Use case:**  
Useful in regression models where you want a general estimate of how far off predictions are.

---

## 3. Mean Squared Error (MSE)

**Definition:**  
Measures the average squared difference between predicted and actual values.

**Formula:**  
MSE = (1/n) * Σ ( y_true - y_pred )²

**Focus:**  
Penalizes larger errors more strongly because of squaring.

**Use case:**  
Popular in regression problems, especially where bigger errors need more penalty.

---

## 📊 Comparison Table

| Loss Function | Focus                  | Effect                          |
|---------------|-----------------------|---------------------------------|
| MaxAE         | Worst case error       | Identifies biggest mistake      |
| MAE           | Average absolute error | Balanced, less sensitive to outliers |
| MSE           | Average squared error  | Penalizes large errors more     |

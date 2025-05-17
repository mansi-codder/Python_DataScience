# 📏 Model Fitness

We now have a way to compare models. But just because a model is the best among those tested does **not** mean that the model is actually good.

For example, for a subset of the data, with our best model of *k = 3*, we calculate the **MSE** (Mean Squared Error) to be **5.0**. Is that good enough?  
What if instead we measure sales in units of individual sales as opposed to thousands? For *k = 3*, the MSE is now **5,004.93**. Is the MSE now good enough?

A graph of sales vs. TV budget with some training data. The *k = 3* model is shown, with an MSE of about 5000.

![Sales vs TV Budget with k=3 Model](image.png)

Clearly, the scale of the data affects the MSE value, making it hard to judge model quality just from the MSE.

---

## 🏆 How Do We Judge Model Fitness?

To answer this, we create a **scale** to compare our model to a very bad model and a very good model:

- The **simplest model** is the average (mean) or naïve model, which always predicts the mean of the target variable. This is the worst possible model that still makes sense.
- The **best possible model** is one where the prediction is identical to the true value for every data point.

---

## 📈 R-squared (Coefficient of Determination)

To put model performance on a scale from 0 to 1, we use a new metric: **R-squared** (R²).

- **R² = 0**: Model is as good as always predicting the mean (naïve model).
- **R² = 1**: Model is perfect; predictions are identical to the true values.
- **R² < 0**: Model is worse than the naïve model (can happen on validation/test data).

> **Watch Out!**  
> Though it is called R‑squared, it is **not** just the square of R.  
> You can get negative R‑squared values if your model performs worse than the mean.

---
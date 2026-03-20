# KFold-Cross-Validation
# 🔄 Model Validation with K-Fold Cross-Validation

This repository explores advanced techniques for evaluating Machine Learning models. By implementing **K-Fold Cross-Validation**, this project demonstrates how to get a reliable estimate of a model's performance by training and testing it on multiple different subsets of the data.

---

## 🛠️ The Validation Stack
* **Python**: Core logic.
* **Scikit-Learn**: For `KFold`, `StratifiedKFold`, and `cross_val_score`.
* **Logistic Regression, SVM, & Random Forest**: Used as base models to compare performance.
* **NumPy**: For calculating the average accuracy across all folds.

---

## 🧠 Key Concepts Implemented

### 1. What is K-Fold?
Instead of a single Train/Test split, the data is divided into **K** equal parts (folds):
* The model is trained **K** times.
* Each time, a different fold is used as the **Test Set**, and the remaining $K-1$ folds are used as the **Training Set**.
* This ensures that every single data point gets to be in the test set exactly once.

### 2. Stratified K-Fold
* Demonstrated how to handle imbalanced datasets by ensuring each fold has the same percentage of samples of each target class as the complete set.

### 3. `cross_val_score`
* Used Scikit-Learn's built-in utility to automate the cross-validation process, making the code cleaner and more efficient.

### 4. Model Comparison
* Used K-Fold to answer the ultimate question: **"Which algorithm is best for this specific dataset?"** by comparing the mean scores of different classifiers.

---

## 📈 Why use Cross-Validation?
* **Reduces Bias:** Prevents a "lucky" or "unlucky" single split from skewing your results.
* **Maximizes Data:** Especially useful for smaller datasets where every row is valuable.
* **Robustness:** Provides a standard deviation of scores, showing how much the model's performance varies.



---

## 🚀 How to Run

1. **Clone the repo:**
   ```bash
   git clone [https://github.com/Manaswi9123/Python-DataScience-Fundamentals.git](https://github.com/Manaswi9123/Python-DataScience-Fundamentals.git)

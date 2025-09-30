
# 🧠 K-Nearest Neighbors (KNN) Classification

This project demonstrates how to implement **K-Nearest Neighbors (KNN)** for classification problems using **Scikit-learn, Pandas, and Matplotlib**.
We use the **Iris dataset** and explore how different values of **K** affect classification performance.

---

## 📌 Objectives

* Understand the KNN algorithm for classification.
* Normalize features before training (since KNN is distance-based).
* Experiment with different values of **K**.
* Evaluate the model using **accuracy** and **confusion matrix**.
* Visualize **decision boundaries** in 2D.

---

## 🛠️ Tools & Libraries

* [Python 3.x](https://www.python.org/)
* [Scikit-learn](https://scikit-learn.org/stable/)
* [Pandas](https://pandas.pydata.org/)
* [Matplotlib](https://matplotlib.org/)
* [NumPy](https://numpy.org/)

Install dependencies:

```bash
pip install scikit-learn pandas matplotlib numpy
```

---

## 🚀 Steps Implemented

1. **Load Dataset** – Used Iris dataset from `sklearn.datasets`.
2. **Preprocess Data** – Standardized features using `StandardScaler`.
3. **Train/Test Split** – Split into training and test sets.
4. **KNN Training** – Trained `KNeighborsClassifier` with different values of **K**.
5. **Evaluation** – Checked accuracy and confusion matrix.
6. **Visualization** – Plotted decision boundaries (using 2 features).

---

## 📊 Results

* Accuracy varies with **K**.
* Best K gives highest accuracy on test data.
* Confusion matrix shows correct vs incorrect classifications.
* Decision boundary visualization shows how KNN separates classes in 2D.

Example confusion matrix (k=5):

```
[[19  0  0]
 [ 0 12  1]
 [ 0  1 12]]
```

---

## 📷 Visualizations

### 🔹 Confusion Matrix

KNN model performance for best **K**.

### 🔹 Decision Boundaries

Decision regions with **2 features (sepal length vs sepal width)**.

---

## 📂 Project Structure

```
├── knn_classification.py   # Main Python script
├── README.md               # Project documentation
```

---

## 🧩 Next Steps

* Use **GridSearchCV** to tune K automatically.
* Try different datasets (e.g., Wine dataset, Breast Cancer dataset).
* Compare KNN with other classifiers (Logistic Regression, SVM, etc.).

---

## 🙌 Author

Developed as part of a **Machine Learning learning task**.



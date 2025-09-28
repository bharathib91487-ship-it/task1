Logistic Regression Classification Workflow
1. Dataset Selection

Used the Breast Cancer Wisconsin Diagnostic dataset (data(1).csv).

Target column: diagnosis

M (Malignant) → 1

B (Benign) → 0

Dropped unnecessary columns: id, Unnamed: 32.

2. Data Splitting and Feature Scaling

Split data into training (80%) and testing (20%) sets using train_test_split.

Standardized features with StandardScaler so that each feature has mean = 0 and variance = 1.

Standardization helps Logistic Regression converge faster and improves performance.

3. Model Training

Initialized and trained a Logistic Regression model:

LogisticRegression(max_iter=10000)


Model learns weights (coefficients) for each feature to predict the probability of malignancy.

4. Model Evaluation

Confusion Matrix: Displays True Positives, True Negatives, False Positives, and False Negatives.

Precision: Fraction of predicted positives that are actually positive.

Recall (Sensitivity): Fraction of actual positives correctly identified.

ROC-AUC: Measures how well the model distinguishes between classes.

ROC Curve: Visualizes the trade-off between True Positive Rate and False Positive Rate.

5. Threshold Tuning & Sigmoid Function

Logistic Regression outputs probabilities using the sigmoid function:

𝜎
(
𝑧
)
=
1
1
+
𝑒
−
𝑧
σ(z)=
1+e
−z
1
	​


By default, predictions use a threshold of 0.5.

Adjusting the threshold (e.g., 0.4 or 0.7) can balance precision and recall depending on the use case.

Thresholding converts probabilities into final class predictions (0 or 1).

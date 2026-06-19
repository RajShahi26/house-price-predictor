# Classification Models, Evaluation Metrics & Handling Imbalanced Data

## Artificial Intelligence & Machine Learning - Task 4

### Project Overview

This project was completed as part of the Artificial Intelligence & Machine Learning Internship Program.

The objective of this task was to build a binary classification model, evaluate its performance using multiple classification metrics, handle class imbalance, and compare different classification algorithms.

The Breast Cancer Wisconsin Dataset from Scikit-learn was used for model development and evaluation.

---

## Objectives

* Understand classification problems
* Build a Logistic Regression classifier
* Evaluate model performance using multiple metrics
* Analyze confusion matrix results
* Interpret Precision, Recall, and F1-Score
* Plot ROC Curve and calculate AUC Score
* Handle class imbalance using class weights
* Compare Logistic Regression with Decision Tree Classifier
* Validate model stability using Cross-Validation

---

## Dataset Information

### Breast Cancer Wisconsin Dataset

The dataset is available in Scikit-learn and is widely used for binary classification tasks.

#### Dataset Statistics

| Attribute      | Value     |
| -------------- | --------- |
| Total Samples  | 569       |
| Total Features | 30        |
| Classes        | 2         |
| Class 0        | Malignant |
| Class 1        | Benign    |

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook
* Git & GitHub

---

## Data Preprocessing

The following preprocessing steps were performed:

* Data loading
* Missing value analysis
* Class distribution analysis
* Train-Test split (80:20)
* Stratified sampling
* Feature scaling using StandardScaler

---

## Models Implemented

### 1. Logistic Regression

Used as the baseline classification model.

```python
LogisticRegression(max_iter=1000)
```

### 2. Decision Tree Classifier

Used for performance comparison.

```python
DecisionTreeClassifier(random_state=42)
```

---

## Evaluation Metrics

The following metrics were used to evaluate model performance:

* Accuracy
* Confusion Matrix
* Precision
* Recall
* F1-Score
* ROC Curve
* AUC Score
* Cross-Validation Accuracy

---

## Results

### Logistic Regression Performance

| Metric                    | Value       |
| ------------------------- | ----------- |
| Accuracy                  | 98.25%      |
| Precision                 | 0.98 - 0.99 |
| Recall                    | 0.98 - 0.99 |
| F1-Score                  | 0.98 - 0.99 |
| AUC Score                 | 0.9954      |
| Cross-Validation Accuracy | 98.02%      |

### Decision Tree Performance

| Metric    | Value       |
| --------- | ----------- |
| Accuracy  | 91.23%      |
| Precision | 0.85 - 0.96 |
| Recall    | 0.90 - 0.93 |
| F1-Score  | 0.89 - 0.93 |

---

## Cross-Validation Results

```text
[0.9670, 0.9780, 0.9670, 1.0000, 0.9890]
```

### Mean Cross-Validation Accuracy

```text
98.02%
```

The cross-validation accuracy is very close to the testing accuracy, indicating strong model stability and good generalization performance.

---

## Handling Class Imbalance

To address class imbalance, Logistic Regression was trained using:

```python
class_weight="balanced"
```

This technique assigns higher importance to minority classes and lower importance to majority classes, helping the model perform fairly across all classes.

---

## ROC Curve and AUC

The ROC Curve was used to evaluate classification performance across different threshold values.

### AUC Score

```text
0.9954
```

An AUC value close to 1 indicates excellent discrimination capability between malignant and benign classes.

---

## Model Comparison

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | 98.25%   |
| Decision Tree       | 91.23%   |

### Final Model Selection

Logistic Regression outperformed the Decision Tree classifier in terms of:

* Accuracy
* Precision
* Recall
* F1-Score
* Stability
* Generalization Capability

Therefore, Logistic Regression was selected as the final model.

---

## Project Structure

```text
Task4/
│
├── AI_ML_Task4_Classification_Evaluation.ipynb
├── Task_4_report.pdf
├── README.md
├── confusion_matrix.png
└── roc_curve.png
```

---

## Conclusion

A binary classification system was successfully developed using the Breast Cancer Wisconsin Dataset.

The Logistic Regression model achieved:

* Accuracy: 98.25%
* AUC Score: 0.9954
* Cross-Validation Accuracy: 98.02%

The model demonstrated excellent predictive performance, strong generalization capability, and superior results compared to the Decision Tree classifier.

---

## Author

**Raj Shahi**

M.Tech – Farm Machinery & Power Engineering
Department of Agricultural and Food Engineering (AGFE)
Indian Institute of Technology Kharagpur (IIT KGP)

---

## License

This project is created for educational and internship learning purposes.

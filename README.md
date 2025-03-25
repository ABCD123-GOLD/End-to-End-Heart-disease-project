# Predicting Heart Disease using Machine Learning

## 1. Problem Definition

**Goal:** Develop a machine learning model to predict whether a patient has heart disease based on clinical attributes.

**Question:** Given a set of clinical parameters, can we accurately classify whether a patient has heart disease?

## 2. Data

**Source:** The dataset comes from the Cleveland Heart Disease dataset available in the **UCI Machine Learning Repository** and **Kaggle**.

**Datasets:**

- `heart-disease.csv`: The main dataset containing medical attributes and the presence (1) or absence (0) of heart disease.

## 3. Evaluation

**Metric:** The model is evaluated using **Accuracy, Precision, Recall, F1-score**, and **ROC-AUC score**.

**Objective:** Achieve at least **95% accuracy** to consider the model successful.

## 4. Features

**Data Dictionary:**

| Feature    | Description                                           |
| ---------- | ----------------------------------------------------- |
| `age`      | Age in years                                          |
| `sex`      | 1 = Male, 0 = Female                                  |
| `cp`       | Chest pain type (0-3)                                 |
| `trestbps` | Resting blood pressure (mm Hg)                        |
| `chol`     | Serum cholesterol in mg/dl                            |
| `fbs`      | Fasting blood sugar > 120 mg/dl (1 = True, 0 = False) |
| `restecg`  | Resting electrocardiographic results (0-2)            |
| `thalach`  | Maximum heart rate achieved                           |
| `exang`    | Exercise-induced angina (1 = Yes, 0 = No)             |
| `oldpeak`  | ST depression induced by exercise                     |
| `slope`    | Slope of the peak exercise ST segment                 |
| `ca`       | Number of major vessels (0-3) colored by fluoroscopy  |
| `thal`     | 3 = Normal, 6 = Fixed defect, 7 = Reversible defect   |
| `target`   | 1 = Heart disease, 0 = No heart disease               |

## 5. Methodology

- **Data Preprocessing:**
  - Handling missing values using imputation.
  - Encoding categorical variables.
  - Feature scaling for improved model performance.
- **Model Selection:**
  - Logistic Regression
  - K-Nearest Neighbors (KNN)
  - Random Forest Classifier
- **Model Training:**
  - Train-test split with cross-validation.
  - Hyperparameter tuning using GridSearchCV.
- **Model Evaluation:**
  - Confusion matrix, Precision, Recall, F1-score, and ROC Curve.

## 6. Visualization

### Cross-Validated Classification Metrics

This visualization showcases the model’s performance across different classification metrics such as **Accuracy, Precision, Recall, and F1-score**. It helps understand the trade-offs between these metrics and ensures that no single metric dominates the evaluation.

![Cross-Validation Metrics](https://github.com/ABCD123-GOLD/End-to-End-Heart-disease-project/blob/main/Images/cross%20validation%20meric.png)

### Feature Importance

The feature importance plot highlights which features contribute most to the model’s predictions. In this case, **thalach (maximum heart rate achieved), cp (chest pain type), ca (number of major vessels), and oldpeak (ST depression induced by exercise)** were among the most significant predictors of heart disease.

![Feature Importance](https://github.com/ABCD123-GOLD/End-to-End-Heart-disease-project/blob/main/Images/Feature%20impoortance.png)

### Confusion Matrix, ROC Curve, and AUC

- **Confusion Matrix:** Displays the number of true positives, true negatives, false positives, and false negatives, giving insights into the model’s classification performance.
  
  ![Model Performance](https://github.com/ABCD123-GOLD/End-to-End-Heart-disease-project/blob/main/Images/AUC%20CURVE.png)

- **ROC Curve & AUC:** The ROC Curve shows the trade-off between true positive and false positive rates, while the **AUC (Area Under the Curve)** score quantifies the model’s ability to distinguish between patients with and without heart disease.

  ![Model Performance](https://github.com/ABCD123-GOLD/End-to-End-Heart-disease-project/blob/main/Images/ROC%20CURVE.png)

## 7. Results and Conclusion

- **Model Performance:** The model achieved **high accuracy and precision**, demonstrating its effectiveness in predicting heart disease.
- **Feature Importance:** Variables such as **thalach, cp, ca, and oldpeak** were among the most significant predictors of heart disease.
- **Overall:** The model provides an accurate and interpretable way to assess heart disease risk.

## 8. Future Improvements

- **Hyperparameter Tuning:** Further fine-tuning models with **Bayesian optimization**.
- **Feature Engineering:** Introduce interaction terms and additional medical parameters.
- **Data Augmentation:** Include more diverse datasets from different medical institutions.
- **Model Selection:** Explore deep learning techniques such as **Neural Networks**.
- **Deployment:** Build an API for real-time heart disease prediction.
- **Error Analysis:** Identify and improve performance on misclassified cases.

---


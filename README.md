# PREDICTION_OF_DIABETICS


# 🩺 Prediction of Diabetes Using Machine Learning

This project applies machine learning techniques to predict whether a person is diabetic based on health-related attributes using the **Pima Indian Diabetes Dataset**. It compares multiple models including Random Forest, Naive Bayes, and K-Nearest Neighbors (KNN) to identify the most accurate classifier.

---

## 📌 About the Project

The goal of this project is to build a predictive model that classifies individuals as diabetic or non-diabetic based on features like glucose level, blood pressure, BMI, insulin level, and more. The data is preprocessed to handle missing values, standardized, and then passed to multiple ML algorithms. Final prediction is based on the best-performing model.

### ✅ Key Features

- Used real-world medical dataset (Pima Indian Diabetes)
- Data cleaning (removing correlated and missing data)
- Data transformation: scaling and imputing
- Trained multiple models: Naive Bayes, Random Forest, KNN
- Evaluated using confusion matrix and classification report
- Final model stored using `pickle` for real-time prediction

---

## 📊 Dataset Description

Features used:
- `num_preg` – Number of pregnancies
- `glucose_conc` – Glucose concentration
- `diastolic_bp` – Diastolic blood pressure
- `insulin` – Insulin levels
- `bmi` – Body mass index
- `diab_pred` – Diabetes pedigree function
- `age` – Age of patient
- `skin` – Skin fold thickness

Target:
- `diabetes` (1 = diabetic, 0 = not diabetic)

---

## 🛠️ Tools & Technologies

- **Python**
- **Pandas**, **NumPy**
- **Matplotlib** (for visualization)
- **Scikit-learn** (ML models and preprocessing)
- **Pickle** (for model serialization)

---

## 🧪 ML Models Used

| Model          | Accuracy (Test Data) | Remarks                |
|----------------|----------------------|-------------------------|
| Naive Bayes    | ~75%                 | Basic probabilistic model |
| Random Forest  | ✅ **Best Accuracy (~83%)** | Preferred model |
| KNN            | ~76%                 | Performs moderately well |

---

## 🚀 How to Run

1. Ensure `pima-data.xlsx` is available in the working directory.
2. Install dependencies:
    ```bash
    pip install pandas numpy matplotlib scikit-learn
    ```
3. Run the Python file:
    ```bash
    python 1_prediction_of_diabetes.py
    ```

---

## 💡 Sample Prediction

Once the model is trained, a new patient's data can be tested:
```python
input_data = [1, 85, 66, 0, 26.6, 0.351, 31, 1.1426]

Prediction: Diabetic or Not Diabetic


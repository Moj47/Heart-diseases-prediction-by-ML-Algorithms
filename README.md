# ❤️ Heart Disease Detection using Machine Learning

This project focuses on detecting heart disease using multiple machine learning algorithms.
The main goal is not only achieving high accuracy, but also making **medically meaningful predictions** 🩺.

---

## 📁 Dataset Information

- 📌 **Total Samples:** 4,241
- 🎯 **Target Variable:** `TenYearCHD`  
  - `0` → No heart disease within 10 years  
  - `1` → Heart disease risk within 10 years  

The dataset contains demographic, behavioral, and medical risk factors related to cardiovascular disease.

### 🔢 Features Description

| Feature | Description |
|------|------------|
| `male` | Gender (1 = Male, 0 = Female) |
| `age` | Age of the patient |
| `education` | Education level |
| `currentSmoker` | Whether the person currently smokes |
| `cigsPerDay` | Number of cigarettes per day |
| `BPMeds` | On blood pressure medication |
| `prevalentStroke` | History of stroke |
| `prevalentHyp` | Hypertension |
| `diabetes` | Diabetes status |
| `totChol` | Total cholesterol |
| `sysBP` | Systolic blood pressure |
| `diaBP` | Diastolic blood pressure |
| `BMI` | Body Mass Index |
| `heartRate` | Heart rate |
| `glucose` | Glucose level |
| `TenYearCHD` | Target label |

---

## 🤖 Models Implemented
- K-Nearest Neighbors (KNN)
- Decision Tree (DT)
- Random Forest (RF)
- Logistic Regression (LR)
- Artificial Neural Network (ANN)

---

## 📊 Evaluation Metrics
Each model was evaluated using:
- Accuracy
- Precision
- Recall
- F1-score  

⚠️ In medical problems, **Recall and F1-score are critical**, since missing a patient with heart disease can have serious consequences.

---

## 🏆 Results Summary

Among all tested models, **Artificial Neural Network (ANN)** showed the best overall performance:

- 🧠 ANN achieved the **highest Recall and F1-score** on the test set.
- 📉 Most traditional ML models reached decent accuracy but failed to detect positive cases.
- ❌ KNN, Decision Tree, and Random Forest had extremely low Recall values.
- ⚖️ Logistic Regression showed good Precision but poor Recall, making it too conservative.

📌 **Final Conclusion:**  
Despite some overfitting, **ANN is currently the most reliable model** for heart disease detection in this project.

---

## 🔍 Why ANN Performed Better
- Captures **non-linear relationships** more effectively
- More flexible decision boundaries
- Better balance between Precision and Recall compared to classical models

---

## 🚀 Future Improvements
Yes… I know 😅 This project is still rough around the edges(It has awful result for now).

Planned updates include:
- 🛠 Better feature engineering
- ⚖️ Handling class imbalance properly
- 🎯 Hyperparameter tuning
- 🔁 Cross-validation
- 🧪 Model optimization and regularization

This repository will be updated as the project evolves.

---
⭐ If you find this project useful or interesting, feel free to star the repository!

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

## 📈 Key Evaluation Results (Test Set)

Since this is a **medical classification problem**, the most important metrics are **Recall** and **F1-score** on the **test set**.
Accuracy alone can be misleading in imbalanced datasets.

### 🔑 Selected Test Metrics

| Model | Accuracy | Precision | Recall | F1-score |
|------|---------|-----------|--------|----------|
| KNN | 0.8333 | 0.5000 | 0.0082 | 0.0161 |
| Decision Tree | 0.8306 | 0.4375 | 0.0574 | 0.1014 |
| Random Forest | 0.8361 | 0.6250 | 0.0410 | 0.0769 |
| Logistic Regression | **0.8402** | **0.8571** | 0.0492 | 0.0930 |
| **ANN** | 0.7992 | 0.3529 | **0.2459** | **0.2899** |

---

## 🥇 Top 3 Models (Based on Medical Relevance)

### 🥇 1. Artificial Neural Network (ANN)
- Highest **Recall** and **F1-score**
- Best at identifying patients with heart disease
- Slight overfitting, but most clinically useful model

### 🥈 2. Decision Tree (DT)
- Better Recall than most classical models
- Simple and interpretable
- Still limited in detecting positive cases

### 🥉 3. Logistic Regression (LR)
- Highest **Precision**
- Very conservative predictions
- Misses many true positive cases (low Recall)

📌 **Final Note:**  
Models with high Accuracy but extremely low Recall (e.g., KNN, Random Forest) are **not suitable** for heart disease detection despite their appealing accuracy scores.
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

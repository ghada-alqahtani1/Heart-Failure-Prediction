<h1 align="center">🫀 Heart Failure Prediction</h1>

<p align="center"><b>Predicting heart disease risk from clinical indicators with classification and clustering</b></p>

<p align="center">
  <img src="assets/model_comparison.png" alt="Decision tree performance comparison" width="680">
</p>

---

## 📁 Project Overview

Heart disease is the leading cause of death worldwide, and it is often diagnosed late. This project uses routine health indicators such as age, blood pressure, cholesterol, and heart rate to identify patients at risk of heart disease, and looks for hidden patient groups that could point to shared risk factors.

---

## 🎯 Objectives

1. Build a classification model that predicts whether a patient has heart disease.
2. Find natural patient groups in the data with clustering.

---

## 🧪 Dataset

- **Source:** [Heart Failure Prediction dataset](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction) on Kaggle
- **Size:** 918 patients, 11 clinical features, 1 target (`HeartDisease`)
- **Class balance:** 508 with heart disease, 410 without
- **Key features:** `Age`, `Sex`, `ChestPainType`, `RestingBP`, `Cholesterol`, `FastingBS`, `MaxHR`, `ExerciseAngina`, `Oldpeak`, `ST_Slope`

---

## 📌 Tools Used

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Scikit-learn and SciPy
- Yellowbrick and Kneed (cluster evaluation)
- Google Colab / Jupyter Notebook

---

## 🔬 Workflow

1. **Exploratory analysis:** summary statistics and charts comparing patients with and without heart disease.
2. **Preprocessing:** replaced 173 invalid zero values in cholesterol and blood pressure with the mean, capped outliers with the IQR method, then applied encoding, normalization, and discretization.
3. **Feature selection:** Chi-square test and correlation analysis; `RestingECG` was dropped.
4. **Classification:** Decision Trees with Information Gain and Gini Index, tested on 70/30, 60/40, and 80/20 splits.
5. **Clustering:** K-Means with K = 2, 3, and 4, evaluated with the silhouette score, WSS, and the elbow method.

---



## 🧠 Conclusion

Simple clinical measurements carry a strong signal for heart disease. A decision tree identifies about 4 in 5 patients correctly while staying easy to interpret, which matters in a medical setting where doctors need to understand why a patient was flagged.

---

## 👩‍💻 Team

- Ghada Alqahtani
- Renad Alowais
- Deema Alfarhoud
- Norah Alshamsan
- Abeer Alsahli

Data Mining course project, King Saud University.

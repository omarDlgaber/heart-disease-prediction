# 🩺 Heart Disease Prediction (Framingham Study)
### Strategic Logistic Regression for High-Recall Medical Diagnosis

## 📌 Project Overview
This project aims to predict the **10-year risk of Coronary Heart Disease (CHD)** using the world-renowned Framingham dataset. As a **Mechatronics Engineer** transitioning into Data Science, I approached this problem by bridging the gap between statistical modeling and clinical necessity.

The primary objective was to build a **safe diagnostic screening tool** that prioritizes patient safety by minimizing missed cases (False Negatives).

---

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Imbalanced-learn (SMOTE).
* **Model:** Logistic Regression (Optimized via GridSearchCV).

---

## 🚀 Key Features & Engineering
To transform a simple linear model into a powerful diagnostic tool, I implemented:
1. **Outlier Management:** Strategic "Capping" to preserve data integrity while reducing noise.
2. **Feature Engineering:** `Pulse Pressure`: Derived from Systolic and Diastolic BP.
   * `Age-BP Interaction`: Capturing the compounding risk of hypertension in older patients.
   * `Polynomial Features`: Modeling the non-linear risk acceleration with `Age^2`.
3. **Strategic Threshold Tuning:** Shifted classification threshold to **0.35** to optimize for **Recall**.

---

## 📊 Final Results
| Metric | Score | Clinical Meaning |
| :--- | :--- | :--- |
| **Recall (Sensitivity)** | **87%** | Successfully identified 87% of all actual high-risk patients. |
| **ROC-AUC** | **0.68** | Strong discriminative power for a linear model on noisy data. |
| **Accuracy** | **49%** | Balanced trade-off to ensure maximum medical safety. |

---

## 🔍 Clinical Interpretation
In heart disease diagnosis, a **False Negative** (telling a sick person they are healthy) is far more dangerous than a **False Positive**. 
* My model successfully reduced missed cases to only **17 out of 129**, ensuring that the vast majority of high-risk individuals are flagged for further clinical testing.

---

## 📂 How to use
1. Clone the repo: `git clone https://github.com/omarDlgaber/heart-disease-prediction.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Run the notebook: `V5_Heart_disease_prediction.ipynb`

---
**Contact:** [LinkedIn](https://www.linkedin.com/in/omar-adel-726407200/?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base%3BIotPy0BzRn%2Bh0RTq1%2BNh3A%3D%3D)

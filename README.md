<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=13&duration=2000&pause=800&color=FF4444&center=true&vCenter=true&width=750&lines=🚨+FRAUD+ALERT+DETECTED;Analyzing+284%2C807+transactions...;Extreme+Imbalance+%E2%80%94+0.17%25+Fraud;Building+Fraud+Detection+Pipeline...;XGBoost+Deployed+%E2%9C%94" alt="Alert Typing SVG" />

<br>

![Banner](https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,50:c0392b,100:e74c3c&height=220&section=header&text=Credit%20Card%20Fraud%20Detection&fontSize=38&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=Imbalanced%20Classification%20with%20Threshold%20Optimisation%20%7C%20Practical%20Exam%20Set%20C&descAlignY=58&descAlign=50&descSize=14)

<br>

[![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge&logo=checkmarx&logoColor=white)](#)
[![Exam](https://img.shields.io/badge/Exam-Practical%20Set%20C-c0392b?style=for-the-badge&logo=academia&logoColor=white)](#)
[![Best Model](https://img.shields.io/badge/Best%20Model-XGBoost%20Tuned-FF6B35?style=for-the-badge&logo=scikitlearn&logoColor=white)](#)
[![Threshold](https://img.shields.io/badge/Optimal%20Threshold-0.644-gold?style=for-the-badge)](#)

<br>

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-EC1C24?style=flat-square)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=flat-square)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![imbalanced-learn](https://img.shields.io/badge/imbalanced--learn-EE4C2C?style=flat-square)

</div>

<br>

---

## 🧠 What is This Project?

> You are a **Junior Data Scientist** at the fraud analytics team of a digital payments company similar to **Paytm or Razorpay**. Every day, millions of transactions flow through the platform — and a small fraction are fraudulent. Missing even a handful of fraud cases costs the company **lakhs of rupees** and damages customer trust.

This project builds a complete, production-grade **fraud detection pipeline** on the real Kaggle Credit Card Fraud dataset — one of the most extreme class imbalance benchmarks in industry ML. The focus goes beyond just building models: it demonstrates **threshold optimisation**, **cost-benefit analysis**, and clear business communication of results.

<div align="center">

```
░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
   284,807 Total Transactions
   ─────────────────────────────────────────────────
   99.83%  Legitimate  ███████████████████████████░
    0.17%  Fraud       ░░░░░░░░░░░░░░░░░░░░░░░░░░░
   ─────────────────────────────────────────────────
   Most extreme imbalance benchmark in industry ML
░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
```

</div>

<br>

---

## 🎯 Learning Objectives

<table>
<tr>
<td width="50%" valign="top">

### 📐 Core ML Concepts
- Why **accuracy is a misleading metric** for fraud detection
- The **Precision-Recall trade-off** and confusion matrix analysis
- **PR-AUC vs ROC-AUC** — which is correct for extreme imbalance
- **Threshold tuning** beyond the default 0.5 cutoff

</td>
<td width="50%" valign="top">

### 🏢 Business Skills
- Assigning **real monetary values** to model errors
- **Cost-benefit analysis** using confusion matrix outputs
- Communicating results to a **non-technical risk manager**
- Understanding when **business-optimal ≠ F1-optimal**

</td>
</tr>
</table>

<br>

---

## 🗺️ Full Project Pipeline

<div align="center">

| Step | Focus | Key Deliverable |
|:---:|:---|:---|
| 🧩 **Step 1** | Theory & Problem Framing | 5 markdown cells explaining accuracy failure, PR tradeoff, imbalance strategies, PR-AUC, and FP vs FN business impact |
| 📊 **Step 2** | Dataset Loading & EDA | 4 plots: class distribution, Amount dist, Time/Hour analysis, V1–V10 correlation heatmap |
| 🔧 **Step 3** | Preprocessing & Feature Engineering | Amount_log, Hour extraction, StandardScaler, train-test split, 3 imbalance strategies |
| 🤖 **Step 4** | Logistic Regression & Random Forest | LR × 3 variants comparison, RF with PR curve and feature importances |
| ⚡ **Step 5** | XGBoost — Full Tuning | Baseline → RandomizedSearchCV → threshold optimisation (F1-optimal + Recall≥0.90) |
| 📈 **Step 6** | Final Model Comparison | 6-row comparison table, all PR curves on one figure, deployment recommendation |
| 💰 **Step 7** | Business Cost-Benefit | Threshold sensitivity table with INR values, net benefit analysis |
| 🚀 **Step 8** | Pipeline & Deployment | sklearn Pipeline → joblib save → load & test on 10 transactions |

</div>

<br>

---

## 📊 Key Results at a Glance

<div align="center">

<table>
<tr>
<td align="center" width="25%">

### 🏆 Best Model
**XGBoost (Tuned)**
<br>
<sub>RandomizedSearchCV optimised</sub>

</td>
<td align="center" width="25%">

### 🎯 F1-Score
**0.9375**
<br>
<sub>At optimal threshold 0.644</sub>

</td>
<td align="center" width="25%">

### 📐 PR-AUC
**0.9297**
<br>
<sub>vs LR baseline 0.813</sub>

</td>
<td align="center" width="25%">

### ✅ Precision
**1.0000**
<br>
<sub>Zero false alarms flagged</sub>

</td>
</tr>
</table>

</div>

<br>

---

## 📈 Model Comparison Table

<div align="center">

| Model | Threshold | Precision | Recall | F1-Score | PR-AUC |
|:---|:---:|:---:|:---:|:---:|:---:|
| Logistic Regression (SMOTE) | 0.50 | 0.309 | 1.000 | 0.472 | 0.813 |
| Random Forest (SMOTE) | 0.50 | 0.933 | 0.824 | 0.875 | 0.875 |
| XGBoost Baseline | 0.50 | 1.000 | 0.824 | 0.903 | 0.897 |
| XGBoost Tuned | 0.50 | 1.000 | 0.882 | 0.938 | 0.930 |
| **XGBoost Tuned (F1-optimal)** | **0.644** | **1.000** | **0.882** | **0.938** | **0.930** |
| XGBoost Tuned (Recall≥0.90) | 0.007 | 0.457 | 0.941 | 0.615 | 0.930 |

</div>

<br>

---

## 💰 Cost-Benefit Analysis

<div align="center">

<table>
<tr>
<td align="center" width="33%">

### 💚 Money Saved
**₹67,500**
<br>
<sub>15 fraud cases caught × ₹4,500</sub>

</td>
<td align="center" width="33%">

### 🔵 Investigation Cost
**₹2,250**
<br>
<sub>15 flagged transactions × ₹150</sub>

</td>
<td align="center" width="33%">

### 💛 Net Benefit
**₹65,250**
<br>
<sub>Per 10,000 transactions</sub>

</td>
</tr>
</table>

</div>

<div align="center">

| Threshold | TP | FP | FN | Money Saved | Investigation Cost | Money Lost | Net Benefit |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 0.10 | 15 | 3 | 2 | ₹67,500 | ₹2,700 | ₹9,000 | ₹64,800 |
| 0.20 | 15 | 2 | 2 | ₹67,500 | ₹2,550 | ₹9,000 | ₹64,950 |
| 0.30 | 15 | 1 | 2 | ₹67,500 | ₹2,400 | ₹9,000 | ₹65,100 |
| 0.50 | 15 | 0 | 2 | ₹67,500 | ₹2,250 | ₹9,000 | ₹65,250 |
| **0.644 (F1-optimal)** | **15** | **0** | **2** | **₹67,500** | **₹2,250** | **₹9,000** | **₹65,250** |

> 💡 **Key Insight:** The F1-optimal threshold and the default 0.5 threshold tie for the highest Net Benefit — proving that **business-optimal ≠ always the lowest threshold**.

</div>

<br>

---

## 🧪 Theory Covered

<details>
<summary><b>📖 Click to expand — Theory Notes from Step 1</b></summary>
<br>

**Why Accuracy Fails for Fraud Detection**
- A model predicting everything as Legitimate gets 99.83% accuracy — but catches zero fraud
- Precision and Recall for the fraud class are both 0 — the model is completely useless despite high accuracy
- PR-AUC and F1-Score must replace accuracy as the primary evaluation metrics

**Precision-Recall Trade-off**
- Lowering the threshold (0.5 → 0.2) flags more transactions as fraud — Recall goes up, Precision goes down
- Raising the threshold flags fewer — Precision improves, but more real fraud is missed
- The optimal threshold depends on the business cost of each type of error

**Three Imbalance Strategies**
- **Class Weights:** Simple, no data modification — but model still sees very few fraud examples
- **SMOTE:** Creates synthetic fraud samples — more varied fraud patterns for the model to learn
- **Undersampling:** Removes majority class rows — fast, but information is lost

**PR-AUC vs ROC-AUC**
- ROC-AUC is inflated by the huge number of True Negatives in extreme imbalance
- PR-AUC focuses entirely on the minority class — cannot be gamed by predicting everything as legitimate

**False Positive vs False Negative Business Impact**
- FP = legitimate customer blocked → ₹150 investigation + customer frustration
- FN = fraud missed → full transaction value lost (₹4,500 average) + chargeback + regulatory risk
- **False Negatives are far more costly** → Recall is the priority metric

</details>

<br>

---

## ⚖️ Imbalance Strategies Explained

<div align="center">

<table>
<tr>
<td align="center" width="33%">

### 🏋️ Class Weights
Tells the model fraud = 580× more important
<br><br>
✅ No data modification<br>
❌ Model still sees few fraud examples

</td>
<td align="center" width="33%">

### 🧬 SMOTE
Generates synthetic fraud samples
<br><br>
✅ Model learns more fraud patterns<br>
❌ Synthetic data ≠ real fraud

</td>
<td align="center" width="33%">

### ✂️ Undersampling
Removes majority class rows
<br><br>
✅ Fast and simple<br>
❌ Throws away real information

</td>
</tr>
</table>

</div>

<div align="center">

**Winner for this dataset: SMOTE** gave the best F1-Score and PR-AUC across Logistic Regression.

</div>

<br>

---

## 🔍 Key Findings from EDA

<div align="center">

<table>
<tr><th>Analysis</th><th>Finding</th></tr>
<tr><td>📊 Class Distribution</td><td>99.83% Legitimate vs 0.17% Fraud — log scale essential to visualise</td></tr>
<tr><td>💵 Transaction Amount</td><td>Fraud spans a wide range — not consistently small amounts; log transform needed</td></tr>
<tr><td>🕒 Time of Day</td><td>Fraud clusters at late night / early morning hours (0–4 AM)</td></tr>
<tr><td>🔗 V-Feature Correlations</td><td>V10, V7, V3 most correlated with fraud; V8 and V6 nearly uncorrelated</td></tr>
<tr><td>🌳 Feature Importances (RF)</td><td>V14 most important (20%), followed by V10, V17, V12, V11</td></tr>
</table>

</div>

<br>

---

## 🚀 Deployment Details

<div align="center">

<table>
<tr><th>Component</th><th>Detail</th></tr>
<tr><td>📦 Pipeline</td><td>sklearn Pipeline wrapping StandardScaler + XGBoost Tuned model</td></tr>
<tr><td>💾 Saved Model</td><td><code>fraud_detection_model.pkl</code> — serialised via joblib</td></tr>
<tr><td>🎯 Optimal Threshold</td><td>0.644 (F1-optimal) — stored alongside the pipeline</td></tr>
<tr><td>🧪 Tested On</td><td>10 sample transactions loaded from pickle — predictions verified</td></tr>
<tr><td>📋 Input Features</td><td>V1–V28 (PCA), Amount_log (log-transformed), Hour (extracted from Time)</td></tr>
</table>

</div>

<br>

---

## 📁 Repository Structure

```
credit-fraud-detection-supervised-learning/
│
├── 📓 FraudDetection_SupervisedLearning.ipynb   ← Fully executed notebook (91 cells)
├── 🤖 fraud_detection_model.pkl                 ← Saved sklearn Pipeline
├── 📄 summary_report.md                         ← Business summary (~400 words)
├── 📋 requirements.txt                          ← All dependencies
└── 📖 README.md                                 ← This file
```

<br>

---

## 📦 Requirements

```
pandas
numpy
matplotlib
seaborn
scikit-learn
imbalanced-learn
xgboost
joblib
jupyter
```

<br>

---

## 👨‍💻 Author

<div align="center">

<img src="https://avatars.githubusercontent.com/u/00000000?v=4" width="100" height="100" style="border-radius:50%;" alt="Author"/>

### **Ayush Isamaliya**
*Data Science & Aspiring ML Engineer*

</div>

---

### 🌐 Connect With Me

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-isamaliya16-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/isamaliya16)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Ayush_Isamaliya-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ayush-isamaliya-686533312/)

</div>

<br>

<div align="center">

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:e74c3c,100:1a1a2e&height=130&section=footer)

**Built as part of the Python Data Science track at Red & White Skill Education**

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=14&duration=4000&pause=1500&color=888888&center=true&vCenter=true&width=550&lines=Thank+you+for+reviewing+this+project!;Star+%E2%AD%90+if+you+found+it+insightful." alt="Footer Typing" />

*Made with ❤️ | Fraud Detection — Practical Exam Set C | Imbalanced Classification | FinTech Analytics*

</div>

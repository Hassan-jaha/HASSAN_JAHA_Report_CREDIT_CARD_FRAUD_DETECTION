# 💳 Credit Card Fraud Detection with Explainable AI (XAI)

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange.svg)
![SHAP](https://img.shields.io/badge/XAI-SHAP-green.svg)

## 📌 Project Overview
In the financial sector, detecting fraud is not just about accuracy—it's about **speed**, **reliability**, and **transparency**. This project develops a high-performance machine learning pipeline to identify fraudulent transactions among 284,807 records, specifically addressing the challenge of extreme class imbalance (only 0.17% fraud).

The unique value of this project is the integration of **SHAP (SHapley Additive exPlanations)** to transform a "Black Box" model into an interpretable system, providing a clear "Reason Code" for every declined transaction.

## 🚀 Key Results (Champion Model)
After comparing multiple architectures, **Pipeline 3 (Advanced Preprocessing + Random Forest)** emerged as the best solution:

* **Recall (Detection Rate):** 0.84 – Successfully capturing 84% of all fraudulent attempts.
* **F1-Score:** 0.88 – A balanced performance between precision and sensitivity.
* **Dimensionality Reduction:** Optimized via **PCA (15 components)** for low-latency real-time inference.
* **Robustness:** Implemented `RobustScaler` to neutralize the impact of extreme transaction outliers.

## 🧠 Explainable AI (XAI) Implementation
To comply with financial regulations and the "Right to Explanation" (GDPR), I utilized **SHAP** to analyze model decisions:

* **Global Importance:** Identified that features like `PC10`, `PC13`, and `PC11` are the strongest indicators of fraud.
* **Local Interpretability:** Generated **Waterfall Plots** for individual transactions to show exactly which factors led to a fraud alert.
* **Trust & Auditability:** The model doesn't just say "Fraud"; it explains **why**.

## 🛠️ Technical Stack
* **Data Handling:** Pandas, NumPy.
* **Machine Learning:** Scikit-Learn (Random Forest, Logistic Regression).
* **Scaling & PCA:** RobustScaler, Principal Component Analysis.
* **Visualization:** Matplotlib, Seaborn, SHAP.

## 📂 Repository Structure
```bash
├── notebooks/          # Jupyter Notebooks with full analysis
├── reports/            # HASSAN_JAHA_Report_CREDIT_CARD_FRAUD_DETECTION.pdf
└── README.md           # Project documentation

👨‍💻 Author
Hassan Jaha Master’s Student in Intelligent Systems for Education (ENS Meknès) Data & AI Developer | Full-Stack Web Expert

Supervised by: Dr. ABDELLAOUI
Institution: École Normale Supérieure (ENS) - Meknès, Morocco.


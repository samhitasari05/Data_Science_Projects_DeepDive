# Scalable Fraud Detection with Geospatial Data

This repository presents a machine learning pipeline for identifying fraudulent financial transactions using supervised learning algorithms. The project focuses on scalability and feature engineering, including the integration of geospatial attributes such as transaction location and time. It demonstrates how machine learning can be applied to detect anomalies in large-scale financial datasets.

This project is independently adapted and extended based on concepts explored in [geekquad/Fraud-Detection](https://github.com/geekquad/Fraud-Detection), with additional restructuring, documentation, and customization.

---

## Project Description

Detecting fraudulent transactions in real-time is a critical challenge for banks, financial institutions, and e-commerce platforms. Fraudulent behavior is often hidden among millions of legitimate transactions and is characterized by severe class imbalance.

This project addresses this challenge by implementing and comparing various supervised ML algorithms while simulating geospatial and temporal features. The objective is to build a scalable fraud detection framework that balances performance, interpretability, and efficiency.

---

## Key Contributions

- Adapted and documented a reusable fraud detection pipeline.
- Incorporated spatial and temporal transaction features for anomaly detection.
- Addressed class imbalance using undersampling and SMOTE.
- Evaluated multiple models (Logistic Regression, Random Forest, XGBoost) using F1-score, ROC-AUC, and precision-recall tradeoffs.
- Outlined future directions including dashboard integration and real-time scoring.

---

## Dataset

- The dataset consists of synthetic credit card transaction records.
- Each row represents a transaction with features such as amount, time, and anonymized attributes.
- A binary target variable indicates whether the transaction is fraudulent.

Geospatial extensions are simulated via:
- Hour-of-day, weekday, and region-based tagging.
- Feature engineering to replicate location-sensitive fraud patterns.

---

## Model Summary

- Algorithms: Logistic Regression, Decision Trees, Random Forest, XGBoost
- Evaluation Metrics: Precision, Recall, F1-Score, ROC-AUC
- Imbalance Handling: Random undersampling, SMOTE
- Feature Engineering: Time-based and synthetic region-based attributes

---

## Folder Structure
├── data/ # Input dataset and preprocessed files
├── notebooks/ # Jupyter notebooks for exploration and modeling
├── models/ # Saved model artifacts
├── scripts/ # Utility scripts (training, evaluation, preprocessing)
├── README.md


---

## Results

- F1-score: Up to 95% on under-sampled training data
- ROC-AUC: 0.98 on Random Forest
- Feature importance and correlation visualized
- Demonstrated impact of time and location-aware features on model accuracy

---

## Setup Instructions

1. Clone the repository:
```bash
git clone https://github.com/samhitasari05/scalable-fraud-detection.git
cd scalable-fraud-detection

2. Install dependencies:
pip install -r requirements.txt

3. Run the Jupyter notebooks or execute training scripts.

Future Work
Integrate dashboards (e.g., Streamlit, Tableau) for fraud monitoring

Connect with real-time streaming data via Kafka or cloud endpoints

Implement geospatial clustering for regional anomaly patterns

Deploy a model API endpoint for live scoring

License and Attribution
This repository builds on open-source materials for educational and portfolio-building purposes.
Base structure inspired by geekquad/Fraud-Detection and adapted under the terms of the MIT License.

Credit Card Fraud Detection using Anomaly Detection

Detecting fraudulent credit card transactions using statistical, unsupervised, clustering-based, and supervised machine learning techniques on a highly imbalanced dataset.

📖 Project Overview

Credit card fraud detection is a classic anomaly detection problem due to the extremely small number of fraudulent transactions compared to legitimate ones.

This project:

Explores multiple anomaly detection techniques

Highlights why accuracy is misleading for imbalanced data

Compares unsupervised models with a supervised baseline

❗ Problem Statement

Fraud transactions make up ~0.17% of the dataset

Traditional models struggle due to class imbalance

The goal is to identify fraud effectively while minimizing false positives

📂 Dataset Description

Type: Credit card transaction data

Target Variable:

0 → Legitimate transaction

1 → Fraudulent transaction

Challenge: Severe class imbalance

🧠 Approach

The notebook evaluates models from four categories:

Statistical Methods

Density-Based Methods

Clustering-Based Methods

Tree-Based & Supervised Models

Each method is assessed for its suitability in fraud detection scenarios.

⚙️ Algorithms Used
🔹 Statistical Anomaly Detection

Z-Score

IQR (Interquartile Range)

4-Sigma Belt

Suitable for simple distributions, but ineffective for complex fraud patterns.

🔹 Density-Based Detection

Local Outlier Factor (LOF)
Detects anomalies based on local density deviation.

🔹 Tree-Based Unsupervised Learning

Isolation Forest ⭐
Efficiently isolates rare observations without distribution assumptions.

🔹 Clustering-Based Detection

DBSCAN
Identifies sparse regions as potential fraud clusters.

🔹 Supervised Learning (Baseline)

Random Forest Classifier ⭐⭐⭐
Trained using labeled data to provide a performance benchmark.

🔍 Key Findings

Accuracy is not reliable for imbalanced datasets

Isolation Forest is the most effective unsupervised approach

Random Forest delivers the best results when labels are available

Fraud detection benefits from multiple detection perspectives

🛠️ Tech Stack

Python 3.x

NumPy

Pandas

Scikit-learn

Matplotlib / Seaborn

Jupyter Notebook

▶️ How to Run
# Clone the repository
git clone https://github.com/your-username/credit-card-fraud-detection.git

# Navigate to the project directory
cd credit-card-fraud-detection

# Install dependencies
pip install -r requirements.txt

# Open the notebook
jupyter notebook analysis.ipynb

Conclusion

Fraud detection is best treated as an anomaly detection problem

Isolation Forest is ideal when labels are missing

Supervised models outperform when labeled data is available

Combining multiple techniques improves real-world reliability

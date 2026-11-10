# 💳 Credit Card Fraud Detection
### 🚨 Catching fraudulent transactions before they slip through.

An end-to-end Machine Learning project that identifies potentially fraudulent credit card transactions using classification algorithms, data analysis, and techniques designed to handle highly imbalanced datasets.

**Machine Learning · Fraud Detection · Imbalanced Classification · Python**

---

## ⚡ The Problem

Credit card fraud detection is not a normal classification problem.

In real-world transaction data, legitimate transactions heavily outnumber fraudulent ones. A model can achieve very high accuracy simply by predicting every transaction as legitimate — while completely failing at its actual job.

**The real challenge:** Detect as many fraudulent transactions as possible while keeping false alarms under control.

This project explores different machine learning approaches to tackle that challenge.

## 🎯 Project Objectives

- Explore and understand highly imbalanced transaction data.
- Identify patterns and relationships through Exploratory Data Analysis.
- Experiment with different techniques for handling class imbalance.
- Train and compare multiple classification algorithms.
- Evaluate models using Precision, Recall, F1-score and Precision-Recall performance.
- Understand the trade-offs between detecting fraud and avoiding false positives.

## 🧠 Models Implemented

| Model | Approach |
|---|---|
| Logistic Regression | Baseline classification |
| Logistic Regression + Class Weights | Cost-sensitive learning |
| Logistic Regression + SMOTE | Oversampling minority class |
| Decision Tree | Rule-based classification |
| Random Forest | Ensemble learning |
| AdaBoost | Boosting |
| XGBoost | Gradient boosting |

## 📊 Model Performance

The following are the recorded test-set results from the project experiments.

| Model | Precision | Recall | F1-score |
|---|---:|---:|---:|
| Logistic Regression | 85.9% | 64.2% | 73.5% |
| Decision Tree | 84.7% | 75.8% | 80.0% |
| Random Forest | 91.1% | 75.8% | 82.8% |
| AdaBoost | 78.3% | 75.8% | 77.0% |
| XGBoost | 92.4% | 76.8% | 83.9% |

**Key observation:** XGBoost achieved the highest recorded F1-score and precision among these models, while Random Forest showed competitive performance. The Decision Tree also provided a useful improvement over the Logistic Regression baseline.

*Note: Re-run the final notebook to verify the displayed results against your latest execution.*

## 🔬 Project Workflow

1. **Data Exploration** — Dataset overview, missing values, duplicates, class distribution and statistical analysis.
2. **Feature Engineering** — Extracting the transaction hour from the time feature.
3. **Data Preprocessing** — Feature scaling and stratified train-test splitting.
4. **Imbalance Handling** — Comparing class weighting and SMOTE.
5. **Model Training** — Training and experimenting with multiple ML algorithms.
6. **Evaluation** — Comparing Precision, Recall, F1-score, Average Precision and confusion matrices.
7. **Visualization** — Class distribution, correlation heatmap, model comparison and Precision-Recall curves.

## 🛠️ Tech Stack

- **Language:** Python
- **Data Analysis:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Imbalanced Learning:** Imbalanced-learn (SMOTE)
- **Boosting:** XGBoost
- **Environment:** Jupyter Notebook

## 📁 Repository Structure

```text
Credit-Card-Fraud-Detection/
│
├── Credit Card Fraud Detection-1.ipynb
├── README.md
└── .gitignore              # Optional
```

The raw dataset is intentionally not included in this repository because of its size.

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd Credit-Card-Fraud-Detection
```

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn xgboost jupyter
```

### 3. Download the dataset

Download the **Credit Card Fraud Detection** dataset from Kaggle:

https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

Place `creditcard.csv` in the same directory as the notebook.

### 4. Run the notebook

```bash
jupyter notebook
```

Open the notebook and execute the cells in order.

## 📌 Key Learnings

Through this project, I explored:

- Why accuracy alone is misleading for imbalanced classification.
- How Precision and Recall influence fraud detection.
- How SMOTE and class weighting address class imbalance.
- How ensemble methods compare with traditional classification algorithms.
- Why Precision-Recall analysis is important when detecting rare events.
- How to compare models using multiple evaluation metrics instead of relying on a single score.

## ⚠️ Limitations & Future Scope

- Explore threshold optimization to balance false positives and false negatives.
- Experiment with additional feature engineering.
- Evaluate model performance on unseen transaction distributions.
- Develop an interactive interface for real-time transaction predictions.

## 👨‍💻 Author

**Darshil Savaliya**

B.Tech Computer Engineering | Machine Learning & AI Enthusiast

---

⭐ If you find this project interesting, feel free to star the repository!

*Built as a hands-on exploration of machine learning techniques for financial fraud detection.*

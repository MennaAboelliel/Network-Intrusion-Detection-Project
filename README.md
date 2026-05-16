# 🔐 Network Intrusion Detection using Machine Learning (UNSW-NB15)

## 📌 Overview
This project is a Machine Learning-based Network Intrusion Detection System (NIDS) built using the **UNSW-NB15 dataset**.  
It aims to classify network traffic as either **normal or attack** using multiple ML models and evaluate the impact of **feature selection** on performance.

The project includes full data preprocessing, exploratory data analysis (EDA), encoding, model training, evaluation, and feature importance analysis.

---

## 🎯 Objective
- Detect network intrusions (cyber attacks)
- Build ML models to classify network traffic
- Compare model performance before and after feature selection
- Analyze most important features in intrusion detection

---

## 📂 Dataset
- Dataset: UNSW-NB15
- Source: Kaggle (Network Security Dataset)
- Target columns:
  - `label` → Normal (0) or Attack (1)
  - `attack_cat` → Attack category

---

## ⚙️ Workflow

### 1️⃣ Data Loading & Setup
- Kaggle API integration
- Dataset extraction and loading into Pandas

---

### 2️⃣ Data Exploration (EDA)
- Dataset shape and structure analysis
- Missing values check
- Label distribution (Normal vs Attack)
- Attack category distribution
- Traffic rate visualization

---

### 3️⃣ Data Cleaning
- Removing duplicates
- Handling missing/invalid values (e.g., service column)

---

### 4️⃣ Feature Engineering
- One-Hot Encoding for categorical variables
- Feature scaling preparation
- Train/Test split (stratified)

---

### 5️⃣ Visualization
- Class imbalance visualization
- Attack category distribution
- Correlation heatmap (top features)
- Traffic behavior analysis

---

## 🤖 Machine Learning Models

### 🔹 Random Forest Classifier
- Baseline model for classification
- Feature importance analysis

### 🔹 Decision Tree Classifier
- Interpretable model
- Used for comparison with Random Forest

---

## 🧠 Feature Selection
- Based on **Random Forest feature importance**
- Top 30 most important features selected
- Comparison before vs after feature selection

---

## 📊 Evaluation Metrics
Models were evaluated using:
- Accuracy Score
- Classification Report (Precision, Recall, F1-score)
- Confusion Matrix
- Cross Validation Score
- ROC Curve & AUC Score

---

## 📈 Results Summary

### 🔹 Before Feature Selection
- Higher dimensional feature space
- Good accuracy but more complexity

### 🔹 After Feature Selection
- Reduced number of features
- Improved efficiency
- Comparable or improved performance in some cases

---

## 📉 Visualizations Included
- Label distribution plot
- Attack category distribution
- Correlation heatmap (pink themed)
- Feature importance comparison
- Confusion matrices (before/after FS)
- ROC curve comparison
- Hyperparameter tuning (n_estimators, max_depth)
- Model performance comparison charts

---

## 🛠️ Technologies Used
- Python 🐍
- Google Colab
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Kaggle API

---

## 🚀 How to Run the Project
1. Open notebook in Google Colab
2. Upload `kaggle.json`
3. Install dependencies:
   ```bash
   pip install kaggle pandas numpy matplotlib seaborn scikit-learn

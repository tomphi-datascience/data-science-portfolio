# 🎯 Customer Segmentation and Value Prediction Using Machine Learning

This project applies both **unsupervised** and **supervised** machine learning techniques to segment customers and predict their future value to a business. The goal is to help businesses target the right customers with the right offers by understanding behavior patterns and estimating lifetime value.

---

## 🧠 Problem Statement

**How can a business group customers based on their behavior and predict which ones are most valuable over time?**

The project addresses two key challenges:
1. **Customer Segmentation** – Identify distinct customer groups using clustering
2. **Customer Value Prediction** – Forecast customer value using regression models

---

## 📊 Dataset

- Source: [[Online Retail K-Means & Hierarchical Clustering]](https://www.kaggle.com/code/hellbuoy/online-retail-k-means-hierarchical-clustering)
- Type: E-commerce transaction dataset
- Size: ~500,000 rows, ~44 MB
- Features: customer ID, purchase amount, frequency, recency, product category, etc.

---

## 🔍 Key Techniques Used

### 🧩 Unsupervised Learning (Segmentation)
- **RFM Analysis** (Recency, Frequency, Monetary value)
- **K-Means Clustering**
- **Silhouette Score** to evaluate clustering
- Customer profiling with visualizations (bar charts, radar plots)

### 📈 Supervised Learning (Value Prediction)
- **Feature Engineering**
- **Logistic Regression, Decision Tree, Random Forest**
- **Model Evaluation**: Accuracy, F1 Score, AUC
- **Hyperparameter Tuning** using GridSearchCV

---

## 🛠️ Tools & Libraries

- Python: pandas, NumPy, scikit-learn, matplotlib, seaborn
- Jupyter Notebook
- Optional: Streamlit for interactive app (coming soon)

---

## 📊 Project Workflow

1. **Data Cleaning**  
   - Handled missing values, duplicate records, and date formatting  
2. **RFM Feature Engineering**  
   - Created Recency, Frequency, and Monetary columns for each customer  
3. **Clustering with K-Means**  
   - Identified optimal number of clusters with Elbow + Silhouette  
   - Labeled customer groups and visualized segment profiles  
4. **Value Prediction Modeling**  
   - Built multiple ML models to classify high-value customers  
   - Compared metrics and selected best-performing model  

---

## 📈 Results

- **Segmentation:** 4 customer segments identified with distinct purchasing behaviors
- **Best Classifier (Random Forest):**  
  - Accuracy: 78%  
  - F1 Score: 0.75  
  - AUC Score: 0.82  

---

## 📁 Folder Structure


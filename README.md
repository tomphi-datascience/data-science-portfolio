# 🏡 Airbnb Price Classifier

This project aims to classify Airbnb listings as **High Price** or **Low Price** using machine learning models. It involves end-to-end steps including data cleaning, feature engineering, visualization, modeling, and evaluation.

---

## 📌 Problem Statement

Given a dataset of Airbnb listings and reviews, can we predict whether a listing will have a **high price** based on its attributes such as reviews, location, host details, and property features?

This classification model could help hosts better price their listings or help Airbnb recommend price ranges to new users.

---

## 📊 Dataset

- Source: [Inside Airbnb - Listings & Reviews](http://insideairbnb.com/get-the-data.html)
- Files used:
  - `listings.csv`
  - `reviews.csv`

The dataset includes variables such as:
- Number of reviews
- Review scores
- Availability
- Room type
- Location
- Amenities

---

## 🛠️ Tools & Technologies

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- scikit-learn (Logistic Regression, SVM, Gradient Boosting)
- Jupyter Notebook
- Feature Engineering & Data Cleaning
- Model Evaluation: Accuracy, F1 Score, ROC AUC
- Hyperparameter Tuning with GridSearchCV

---

## 🔍 Key Steps

1. **Data Cleaning**  
   - Merged listings and reviews datasets
   - Removed high-cardinality and irrelevant columns
   - Handled missing values and outliers

2. **Feature Engineering**  
   - Converted categorical features
   - Scaled numerical variables
   - Created binary target variable (high vs. low price)

3. **Modeling**  
   - Trained and compared three ML models:
     - Logistic Regression
     - Support Vector Machine (SVM)
     - Gradient Boosting Classifier
   - Performed hyperparameter tuning
   - Selected best model based on F1 Score and ROC AUC

4. **Evaluation**  
   - Visualized confusion matrix and ROC curve
   - Compared models using classification metrics

---

## 📈 Results

| Model                  | Accuracy | F1 Score | ROC AUC |
|------------------------|----------|----------|---------|
| Logistic Regression    | 56%      | 0.55     | 0.59    |
| SVM                    | 58%      | 0.57     | 0.60    |
| Gradient Boosting (best)| **60%**  | **0.59** | **0.63** |

---

## 📁 Folder Structure


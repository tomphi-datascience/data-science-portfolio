# 📰 Fake News Detection Using Machine Learning & NLP

This project uses **Natural Language Processing (NLP)** and **supervised machine learning** to classify news articles as **real** or **fake**. It aims to combat misinformation by providing an automated way to evaluate the credibility of textual content.

---

## 🧠 Problem Statement

**Can we automatically identify whether a news article is real or fake based on its content?**

The project solves this binary classification problem using text vectorization and multiple ML algorithms to determine the authenticity of news articles.

---

## 📊 Dataset

- Source: [[Fake and Real News Dataset – Kaggle]](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset)
- Type: News article dataset with labeled samples
- Size: ~50,000 articles
- Features: title, text content, label (FAKE or REAL)

---

## 🔍 Key Techniques Used

### 📄 Text Preprocessing (NLP)
- Lowercasing, punctuation removal, stopword filtering
- TF-IDF Vectorization to convert text into numerical features

### 🤖 Machine Learning Models
- **Logistic Regression**
- **Naive Bayes**
- **XGBoost**

### 🧪 Model Evaluation
- Accuracy, F1 Score, ROC AUC
- Confusion matrix and classification reports

---

## 🛠️ Tools & Libraries

- Python: pandas, NumPy, scikit-learn, matplotlib, seaborn
- NLP: TF-IDF (TfidfVectorizer)
- Streamlit (for web deployment)
- Jupyter Notebook
- Git, GitHub

---

## 🔄 Project Workflow

1. **Data Loading & Cleaning**  
   - Merged real and fake datasets  
   - Dropped irrelevant fields like subject, date  
   - Combined title and content into one feature column  

2. **Text Vectorization**  
   - Applied TF-IDF transformation to the cleaned text data  

3. **Model Training**  
   - Trained Logistic Regression, Naive Bayes, and XGBoost models  
   - Tuned hyperparameters and evaluated using cross-validation  

4. **Web App Deployment**  
   - Built an interactive UI using Streamlit  
   - Allows users to input custom text and get real-time predictions  

---

## 📈 Results

- **Logistic Regression**: Accuracy = 99.6%, ROC AUC = 99.9%  
- **Naive Bayes**: Accuracy = 95.6%  
- **XGBoost**: Accuracy = 99.8%, ROC AUC = 99.9%  
- All models showed high performance on TF-IDF-transformed data

---

## 📁 Folder Structure
```text fake-news-detector/ │ ├── app.py # Streamlit web app ├── notebook.ipynb # Development notebook ├── model/ # Saved models and pipelines ├── data/ # Dataset or link to source ├── requirements.txt # Project dependencies ├── README.md # Project overview └── .gitignore # Files to exclude from Git ```


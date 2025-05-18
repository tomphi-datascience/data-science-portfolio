# 📰 Fake News Detection Using Machine Learning & NLP

This project uses **Natural Language Processing (NLP)** and **supervised machine learning** to classify news articles as **real** or **fake**. It aims to combat misinformation by providing an automated way to evaluate the credibility of textual content.

---

## 🧠 Problem Statement

**Can we automatically identify whether a news article is real or fake based on its content?**

This binary classification project uses vectorized text and multiple machine learning models to detect fake news with high accuracy.

---

## 📊 Dataset

- **Source**: [Fake and Real News Dataset – Kaggle](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset)  
- **Type**: News article dataset with labeled samples  
- **Size**: ~50,000 articles  
- **Features**: Title, full text, label (FAKE or REAL)

---

## 🔍 Key Techniques Used

### 📄 Text Preprocessing
- Lowercasing, punctuation removal, stopword filtering
- Combined `title` and trimmed `text` into a single input feature
- TF-IDF Vectorization for numerical representation

### 🤖 Machine Learning Models
- **Logistic Regression**
- **Naive Bayes**
- **XGBoost**
- **Random Forest**

### 🧪 Model Evaluation
- Accuracy, F1 Score, ROC AUC
- Confusion matrix and classification reports

---

## 🛠️ Tools & Libraries

- Python: `pandas`, `NumPy`, `scikit-learn`, `matplotlib`, `seaborn`  
- NLP: `TfidfVectorizer` (TF-IDF)  
- Deployment: `Streamlit`  
- Environment: Jupyter Notebook, Git, GitHub

---

## 🔄 Project Workflow

1. **Data Cleaning**  
   - Merged real and fake datasets  
   - Dropped unused fields (`subject`, `date`)  
   - Created new feature column by combining `title` and `text`

2. **Text Preprocessing & Vectorization**  
   - Cleaned and vectorized text using TF-IDF

3. **Model Training & Evaluation**  
   - Trained Logistic Regression, Naive Bayes, Random Forest, and XGBoost  
   - Evaluated using cross-validation and performance metrics

4. **Deployment**  
   - Built an interactive Streamlit app for real-time text classification

---

## 📈 Results

| Model               | Accuracy | ROC AUC |
|--------------------|----------|---------|
| Logistic Regression| 99.6%    | 99.9%   |
| Naive Bayes        | 95.6%    | 99.2%   |
| XGBoost            | 99.8%    | 99.9%   |
| Random Forest      | 99.7%    | 99.8%   |

All models performed strongly on TF-IDF-transformed data, with XGBoost and Logistic Regression achieving near-perfect scores.

---

## 📁 Folder Structure

```text
fake-news-detector/
│
├── app.py                # Streamlit web app
├── notebook.ipynb        # Development notebook
├── model/                # Saved models and pipelines
├── data/                 # Dataset or link to source
├── requirements.txt      # Project dependencies
├── README.md             # Project overview
└── .gitignore            # Files to exclude from Git```

---

## 🔍 Future Improvements

- Add **lemmatization** and **named entity recognition (NER)** to enhance text understanding
- Train on **larger-scale** or **multilingual** news datasets for broader generalization
- Improve the **Streamlit UI/UX** with clearer feedback and styling
- Integrate with **real-time news APIs** (e.g., NewsAPI, GNews) for live article classification
- Add **explainability tools** like SHAP or LIME to visualize model reasoning
- Deploy on the cloud (e.g., **Streamlit Cloud**, **Heroku**, or **AWS**) for public access


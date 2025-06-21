# 🐦 Twitter Sentiment Analysis using Sentiment140

This project performs binary sentiment classification (positive or negative) on tweets using the **Sentiment140** dataset. It uses natural language processing (NLP) techniques and a Logistic Regression model to identify sentiment in tweets.

## 📘 Project Overview

- **Project Title**: Twitter: Sentiment Analysis  
- **Course**: Python Programming Skill-Based Laboratory (Semester IV)  
- **Guide**: Mr. Raunak Joshi  
- **Team Members**:
  - Punit Ayare  
  - Pankaj Bhandari  
  - Devendra Gurav  

---

## 📂 Dataset: Sentiment140

- **Source**: [Kaggle - Sentiment140](https://www.kaggle.com/datasets/kazanova/sentiment140)
- **Records**: 1.6 million tweets  
- **Fields**:
  - `target`: Sentiment label (0 = negative, 4 = positive)
  - `text`: Tweet content
  - `date`, `query`, `user`: Metadata (not used in modeling)

---

## 🧠 Workflow

### 🔹 Data Preprocessing
- Convert to lowercase
- Remove:
  - URLs
  - Mentions (@username)
  - Hashtags
  - Special characters and punctuation
- Tokenization
- **Negation Handling** (e.g., "not good" → "not_good")
- Remove stopwords (custom list that retains negation words)

### 🔹 Feature Extraction
- TF-IDF Vectorizer

### 🔹 Model
- **Algorithm**: Logistic Regression  
- **Evaluation Metrics**:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Confusion Matrix

---




## 📈 **Results**

**Model**: Logistic Regression

**Metrics**:
- **Accuracy**: 85%
- **Precision**: 84%
- **Recall**: 85%
- **F1 Score**: 84.5%


**Observations**:
- Preprocessing, especially **negation handling**, significantly improves accuracy.
- **TF-IDF** helps in extracting meaningful features from tweets.
- **Logistic Regression** offers fast training and solid baseline results.

---

## 📚 **References**

- [**Sentiment140 Dataset on Kaggle**](https://www.kaggle.com/datasets/kazanova/sentiment140)
- [**NLTK Documentation**](https://www.nltk.org/)
- [**Scikit-learn User Guide**](https://scikit-learn.org/stable/user_guide.html)



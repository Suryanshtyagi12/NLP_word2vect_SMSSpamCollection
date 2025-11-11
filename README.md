# 📩 SMS Spam Detection using Word2Vec and Avg Word2Vec

This project focuses on detecting spam messages in SMS text data using **Word2Vec** and **Average Word2Vec** embeddings.  
The dataset used is the popular **[SMSSpamCollection](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection)** dataset from the UCI Machine Learning Repository.

---

## 🧠 Project Overview

The goal of this project is to classify SMS messages as **Spam** or **Ham (Not Spam)** using vectorized text representations.

To achieve this, we:
1. Preprocess the text messages.
2. Convert words into numerical representations using:
   - **Word2Vec embeddings**
   - **Average Word2Vec embeddings**
3. Train machine learning models on these embeddings.
4. Evaluate performance using classification metrics.

---

## 📊 Dataset

**Dataset Name:** SMSSpamCollection  
**Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection)  
**Description:**  
A collection of SMS messages labeled as **spam** or **ham**.

| Label | Example Message |
|--------|-----------------|
| ham | "Hey, are you coming to the party tonight?" |
| spam | "Congratulations! You’ve won a $1000 gift card. Click here to claim." |

---

## ⚙️ Workflow

### 1. Data Preprocessing
- Convert text to lowercase  
- Remove punctuation and special characters  
- Tokenize sentences into words  
- Remove stopwords and perform lemmatization  

### 2. Feature Extraction
#### a. Word2Vec
We train a Word2Vec model to create dense vector representations of words.  
Each word is represented as a high-dimensional numeric vector based on its context in the text.

#### b. Average Word2Vec
Each SMS message is represented as the **average** of its word vectors — this creates a single fixed-length vector per message.

### 3. Model Training
We experiment with classifiers like:
- Logistic Regression  
- Random Forest  
- Naive Bayes  

### 4. Evaluation
We use standard classification metrics:
- Accuracy  
- Precision  
- Recall  
- F1 Score  

---

## 🧩 Technologies Used

| Tool / Library | Purpose |
|-----------------|----------|
| Python | Programming language |
| pandas, numpy | Data handling and numerical operations |
| gensim | Word2Vec embeddings |
| scikit-learn | Model training and evaluation |
| nltk | Text preprocessing and tokenization |

---

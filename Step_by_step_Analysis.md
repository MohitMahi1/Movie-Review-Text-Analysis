# 📊 How to Do Data Analysis — Step-by-Step Guide

This section explains the **general workflow** that any Data Analyst or Data Scientist follows when analyzing a dataset.  
Follow these steps whenever you start a new analysis project.

---

##  Step 1 — Understand the Problem

Before touching the data:

- What is the business question?
- What do we want to predict / classify / analyze?
- Who will use the output?

Example question:  
**“Given a movie review, predict whether it's positive or negative.”**

---

##  Step 2 — Gather the Data

Data can come from:

- CSV / Excel files  
- SQL / NoSQL databases  
- APIs  
- Web scraping  
- Cloud storage

Make sure to inspect the data first using:

```python
df.head()
df.info()
df.describe()
```

---

##  Step 3 — Data Cleaning

The most important step!

- Handle missing values  
- Convert text to lowercase  
- Remove duplicates  
- Remove URLs  
- Remove HTML tags  
- Fix spelling errors  
- Remove punctuations & special characters  
- Remove extra spaces  

Clean data → Better analysis → Better model accuracy.

---

##  Step 4 — Data Preprocessing

Transform data into usable form:

### ✔ Tokenization  
Split sentences into words.

### ✔ Stopword Removal  
Remove words like *the, a, is, and*.

### ✔ Stemming / Lemmatization  
Convert words to their base form.

### ✔ Encoding & Scaling (for numerical data)
- Label Encoding
- One-Hot Encoding  
- StandardScaler / MinMaxScaler

---

##  Step 5 — Exploratory Data Analysis (EDA)

Here you try to **understand patterns** in the data.

Visualize:

- Distributions (histograms, KDE plots)
- Correlations (heatmap)
- Relationships (scatter plots)
- Count plots
- Word clouds (for text data)
- Bigram / trigram frequency

Ask questions like:

- What are the most common words?
- Which sentiment has longer reviews?
- Are there any outliers?

---

##  Step 6 — Feature Engineering

Create new useful features:

- Review length  
- Word count  
- Bigram frequency  
- Sentiment-based features  
- Text embeddings  

Good features → good model.

---

##  Step 7 — Vectorization (Only for Text Data)

ML models cannot read text → convert to numbers.

Common methods:

- **Bag of Words**
- **TF-IDF**
- **Word2Vec**
- **GloVe**
- **BERT embeddings**

---

##  Step 8 — Model Building

Choose models based on problem type:

### Classification:
- Logistic Regression  
- Naïve Bayes  
- SVM  
- Random Forest  
- XGBoost  
- Neural Networks  

Split data:

```python
train_test_split(X, y, test_size=0.2)
```

Train → Test → Evaluate.

---

##  Step 9 — Model Evaluation

Check:

- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion matrix  
- ROC–AUC curve  

Ensure the model is not overfitting or underfitting.

---

## Step 10 — Deployment (Optional)

Deploy using:

- Flask / FastAPI  
- Streamlit  
- Django  
- AWS / GCP / Azure  

Or make a REST API so others can use your model.

---

# 🎯 Summary

**This is the universal 10-step process for any data analysis or machine learning project:**

1. Understand the problem  
2. Gather data  
3. Clean the data  
4. Preprocess  
5. EDA  
6. Feature engineering  
7. Vectorization  
8. Model building  
9. Evaluation  
10. Deployment  

---

This guide can be used for **any dataset**, not just text or sentiment analysis.

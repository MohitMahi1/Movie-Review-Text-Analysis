# Movie Reviews Text Cleaning & Preprocessing (NLP Pipeline)

This project focuses on preparing a movie-review dataset for a Sentiment Analysis Model.
The main objective of the team is to build a machine-learning model that predicts whether a review is Positive or Negative.

My specific responsibility in the project is complete Data Cleaning, Preprocessing, and EDA, ensuring that the dataset is fully ready for ML model building.

The dataset contains **two columns**:
- **review** -- the text written by the user
- **sentiment** -- either *positive* or *negative*

My responsibility in this project was **data cleaning**,
**preprocessing**, **EDA**, and **vectorization** before the
model-building step.

------------------------------------------------------------------------

## 1. Data Gathering

The dataset was collected and loaded successfully (`IMDB Dataset.csv`).

------------------------------------------------------------------------

##  2. Data Cleaning

The main purpose of data cleaning is to remove noise so the
machine-learning model learns meaningful patterns.

The following steps were performed:

### **a. Text Normalization**

-   Converted all text to **lowercase**
-   Removed **leading & trailing spaces**

### **b. Noise Removal**

-   Removed **HTML tags**\
-   Removed **URLs**
-   Expanded **abbreviations** (e.g., *you'll → you will*)
-   Applied **spelling correction**
-   Removed **punctuations** (e.g., `! ? : .`)
-   Removed **special characters**

These steps ensure the text becomes uniform and easier for the model to
analyze.

------------------------------------------------------------------------

##  3. Data Preprocessing

After cleaning, we prepare the text for machine learning algorithms.

### **a. Tokenization**

Breaking sentences into individual words (*tokens*).

### **b. Stopwords Removal**

Removing unimportant words like:\
`['is', 'am', 'are', 'the', 'and', 'I', 'you']`

### **c. Stemming**

Converting words into their root form:\
- *went, going, goes → go*

This reduces vocabulary size and improves model performance.

------------------------------------------------------------------------

##  4. Exploratory Data Analysis (EDA)

EDA was performed to understand the structure and patterns in the
dataset.

Some visualizations include: - Distribution of character length -
Comparison of positive vs negative reviews - Bigram frequency
visualization - Token length distribution\
- Other text-based statistical observations

------------------------------------------------------------------------

##  5. Feature Engineering

Created additional helpful features such as: - Character length of
review\
- Total number of tokens\
- Number of stopwords\
- Bigram frequency\
(Only if needed for model performance)

------------------------------------------------------------------------

##  6. Vectorization

Machine learning algorithms cannot understand text, so we convert text
into numbers.

Two types of vectorization were performed:

### **a. Bag of Words (BoW)**

Represents the frequency of each word in the text.

### **b. TF-IDF**

Term Frequency -- Inverse Document Frequency\
Helps identify the importance of a word in a document compared to the
whole dataset.

This creates high‑dimensional numerical representation of text which is
used for training ML models.

------------------------------------------------------------------------

#  Libraries Used

- **Python**
- **Pandas**
- **NumPy**
- **NLTK**
- **TextBlob**
- **scikit-learn**
- **Matplotlib / Seaborn**

------------------------------------------------------------------------
## 🎯 Final Goal

To enable a machine learning model to accurately classify whether a
given movie review is **positive** or **negative** based on the cleaned,
processed, and vectorized text.

------------------------------------------------------------------------

## 📁 Dataset Used

`IMDB Dataset.csv` (Movie Reviews Dataset)

------------------------------------------------------------------------

## ✨ Conclusion

This NLP pipeline establishes a structured and optimized approach to
prepare raw text data for sentiment analysis models.\
Clean and well‑processed data ensures better accuracy and generalization
in the final model.

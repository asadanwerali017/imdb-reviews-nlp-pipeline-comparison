# IMDb Sentiment Analysis & Topic Modeling – NLP Pipeline Comparison

This project analyzes IMDb movie reviews using Natural Language Processing (NLP).  
I have compared multiple preprocessing pipelines for sentiment classification and explored topic modeling techniques.

---

## Project Goals

- Building a sentiment classification model for movie reviews
- Comparing different preprocessing pipelines:
  - Unigrams vs bigrams
  - Stopword removal
  - Lemmatization (spaCy)
- Evaluating how preprocessing affects accuracy
- Performing topic modeling using LDA and NMF

---

## Methods

### Sentiment Classification
- TF-IDF vectorization
- Logistic Regression classifier
- Pipelines tested:
  - Base cleaning + unigrams
  - Base cleaning + unigrams + bigrams
  - Stopwords removed (negations preserved) + bigrams
  - spaCy lemmatization + bigrams

### Topic Modeling
- LDA with CountVectorizer
- NMF with TF-IDF

---

## Results

| Pipeline | Description | Accuracy |
|---------|-------------|----------|
| P1 | Base cleaning + unigrams | 0.9005 |
| P2 | Base cleaning + unigrams + bigrams | 0.9062 |
| P3 | Stopwords removed (keep NOT) + bigrams | 0.9007 |
| P4 | spaCy lemmatization + bigrams | 0.8964 |

---

## Key Findings

- Bigrams significantly improved sentiment classification accuracy.
- Removing stopwords reduced performance slightly.
- Lemmatization did not improve results for this dataset.
- NMF produced more interpretable topics than LDA for IMDb reviews.

---

## Technologies Used

- Python
- scikit-learn
- spaCy
- pandas
- NumPy
- Jupyter Notebook

---

## Author
Asad Anwer Ali Andani

Asad

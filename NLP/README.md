# Natural Language Processing (NLP)

This folder contains my learning and implementation of fundamental **Natural Language Processing (NLP)** techniques and a final Machine Learning project for **Emotion Classification**.

The implementations cover basic text representation techniques such as **One-Hot Encoding, Bag of Words, and TF-IDF**, followed by a practical NLP classification project using **Multinomial Naive Bayes** and **Logistic Regression**.

---

## 📂 Contents

### 1. One-Hot Encoding

Implementation of **One-Hot Encoding** for representing text as numerical vectors.

* Converts words into binary vectors
* Each word is represented by a unique position
* Demonstrates the basic concept of numerical text representation

---

### 2. Bag of Words (BoW)

Implementation of the **Bag of Words** model.

* Creates a vocabulary from the text corpus
* Represents documents based on word occurrence
* Ignores the order of words
* Uses word frequency as features

---

### 3. TF-IDF

Implementation of **Term Frequency–Inverse Document Frequency (TF-IDF)**.

TF-IDF assigns importance to words based on:

* How frequently a word occurs in a document
* How common or rare the word is across the entire corpus

It helps reduce the importance of very common words while giving higher importance to informative words.

---

## 🚀 Final Project: Emotion Classification

The final project applies NLP techniques to an **Emotion Dataset from Kaggle** to classify text into different emotion categories.

### Objective

Build a Machine Learning model that can understand the emotional content of a given text and predict its corresponding emotion.

### Dataset

The project uses an **Emotion Dataset obtained from Kaggle** containing text samples labeled with their respective emotions.

The dataset is preprocessed and transformed into numerical features using:

* Count Vectorizer
* TF-IDF Vectorizer

---

## 🧠 Machine Learning Models

Two classification algorithms were trained and evaluated:

### Multinomial Naive Bayes

Multinomial Naive Bayes is well suited for text classification problems because it works effectively with discrete features such as word counts and TF-IDF values.

### Logistic Regression

Logistic Regression is used as a linear classification algorithm for predicting the emotion associated with a given text.

---

## 🔬 Experiments

The project compares different combinations of vectorization techniques and classification algorithms.

| Feature Extraction | Model                   |
| ------------------ | ----------------------- |
| Count Vectorizer   | Multinomial Naive Bayes |
| Count Vectorizer   | Logistic Regression     |
| TF-IDF Vectorizer  | Multinomial Naive Bayes |
| TF-IDF Vectorizer  | Logistic Regression     |

This allows comparison of how different text representation techniques affect classification performance.

---

## 🔄 NLP Pipeline

```text
Raw Text
   ↓
Text Preprocessing
   ↓
Feature Extraction
   ↓
Count Vectorizer / TF-IDF
   ↓
Train-Test Split
   ↓
Machine Learning Model
   ↓
Prediction
   ↓
Model Evaluation
```

---

## 🛠️ Technologies & Libraries

* Python
* Pandas
* NumPy
* Scikit-learn
* Jupyter Notebook

---

## 📊 Key Learnings

Through this NLP module, I learned:

* How text is converted into numerical representations
* Working of One-Hot Encoding
* Working of the Bag of Words model
* Working of TF-IDF
* Difference between Count Vectorization and TF-IDF
* Applying NLP preprocessing techniques
* Using NLP features for Machine Learning
* Text classification using Multinomial Naive Bayes
* Text classification using Logistic Regression
* Comparing different feature extraction and classification combinations

---

## 🎯 Conclusion

This NLP module provides a foundation for understanding how **text data can be transformed into numerical features and used with Machine Learning algorithms**.

The final Emotion Classification project demonstrates the complete workflow from **raw text preprocessing to feature extraction, model training, prediction, and evaluation**.

---

## 📌 Future Improvements

* Implement Word Embeddings
* Explore Word2Vec and GloVe
* Implement advanced text preprocessing
* Experiment with Deep Learning models
* Explore Transformer-based models such as BERT
* Improve emotion classification performance

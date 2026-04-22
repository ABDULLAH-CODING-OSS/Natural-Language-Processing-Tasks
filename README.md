# 📌 NLP Spam Classification Project

## 📖 Overview

This project implements a complete Natural Language Processing (NLP) pipeline to classify SMS messages as **Spam** or **Ham (non-spam)**. It covers data analysis, text preprocessing, feature extraction, and machine learning model training.

---

## 📊 Dataset

* **Dataset:** SMS Spam Collection Dataset
* **Samples:** 5572 messages
* **Classes:** Spam, Ham
* **Source:** https://archive.ics.uci.edu/ml/datasets/sms+spam+collection

---

## 🔍 Workflow

### 1️⃣ Exploratory Data Analysis

* Dataset structure and size
* Class distribution (imbalanced dataset)
* Vocabulary analysis
* Sample message inspection

---

### 2️⃣ Text Preprocessing

* Lowercasing
* Removal of special characters
* Tokenization
* Stopword removal
* Lemmatization
* Creation of processed text (`final_text`)

---

### 3️⃣ Feature Engineering

* **Bag of Words (BoW)**
* **TF-IDF**
* **Bigram Model**

---

### 4️⃣ Model Training

* Algorithm: **Naive Bayes**
* Features used: BoW, TF-IDF, Bigrams

---

## 📈 Results

| Method  | Accuracy | Observation                            |
| ------- | -------- | -------------------------------------- |
| TF-IDF  | ~97%     | Best overall performance               |
| BoW     | ~96%     | Higher recall for spam                 |
| Bigrams | ~76%     | High dimensionality, lower performance |

---

## 🧠 Key Insights

* Preprocessing reduces noise and improves feature quality
* TF-IDF provides the best balance between precision and accuracy
* BoW captures spam effectively but may increase false positives
* Bigrams increase feature size significantly and reduce efficiency

---

## 🚀 Example Prediction

```python
predict_message("Congratulations! You have won a free prize!")
```

---

## 🛠️ Technologies Used

* Python
* pandas
* nltk
* scikit-learn

---

## 📌 Conclusion

This project demonstrates how preprocessing and feature engineering impact NLP model performance and highlights trade-offs between different feature representation techniques.

---

## 👤 Author

Abdullah Javed
University of Management and Technology

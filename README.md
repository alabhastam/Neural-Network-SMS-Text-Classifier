# 📱 SMS Spam Classifier

This project builds a machine learning model to classify SMS messages as either **ham** (normal) or **spam** (unsolicited advertising). It uses the [SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset), split into training and validation `.tsv` files.

---

## 📂 Dataset

The data is provided in two `.tsv` (tab-separated values) files:

- `train.tsv` – training data
- `valid.tsv` – validation data

Each row contains:
- `label`: `ham` or `spam`
- `text`: the SMS message content

---

## 📊 Model

The classification model is a **scikit-learn pipeline** consisting of:

1. `TfidfVectorizer` – Converts text into numerical features based on word importance
2. `MultinomialNB` – A Naive Bayes classifier optimized for text classification

---


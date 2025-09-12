

# Urdu Sentiment Labeling & Analysis

This repository contains the **labeling and sentiment analysis part** of a larger NLP project. The main focus is on **Urdu text processing and sentiment classification**.
 Full methodology and evaluation are explained in [SentimentReport.pdf](./SentimentReport.pdf).
## 📌 Overview

* Extracted sentences from **YouTube transcripts**.
* Assigned sentiment **labels (Positive / Negative)** and removed *neutral* samples.
* Translated sentences into **Urdu** for building an Urdu-focused dataset.
* Performed **sentiment analysis** using classical Machine Learning models.


## Dataset

- Source: YouTube drama transcripts.  
- Size: **40,200 labeled sentences**.  
- Split:  
  - **Train**: 32,160  
  - **Test**: 8,040  

Example record:

| Sentence Number | Drama Name | Episode | Youtube Link | Sentence (Eng) | Sentence (Urdu) | Sentiment |
|-----------------|------------|---------|--------------|----------------|-----------------|-----------|
| 1 | Fitoor | 38 | https://youtu.be/gY6ayspZuZQ | I have really hurt you, | میں نے تمہیں واقعی تکلیف دی ہے، | N |

---

## Models Used

The following models were trained on TF-IDF features:

- ✅ Logistic Regression  
- ✅ Naive Bayes  
- ✅ Support Vector Machine (SVM)  
- ✅ XGBoost  
- ✅ LightGBM  

---

## Results

| Model                | Accuracy |
|-----------------------|----------|
| Logistic Regression   | 0.93 |
| Naive Bayes           | 0.89 |
| SVM                   | 0.94 |
| XGBoost               | 0.90 |
| LightGBM              | 0.90 |

📊 Detailed classification reports are included in the console output and the report PDF.

---

## Predictions on Sample Urdu Sentences

Example predictions:

```text
Sentence: "یہ پروڈکٹ واقعی بہت شاندار ہے" → P  
Sentence: "مجھے یہ بالکل پسند نہیں آیا" → N  
Sentence: "سروس بہت اچھی تھی" → P  
Sentence: "پیسے ضائع کیے، کوئی فائدہ نہیں ہوا" → N  
```

## 🧩 Key Learning Goals

* Understanding how **text classification** works in practice.
* Applying **TF-IDF vectorization** to convert text into features.
* Using **simple ML models** (e.g., Logistic Regression, Naïve Bayes, SVM) for sentiment classification.
* Gaining hands-on experience with the **ML workflow** (data preprocessing → feature extraction → training → evaluation).

## 📂 Repository Contents

* `SentimentReport.pdf` → Contains **labeling and analysis results** with explanations.
* Code files → Scripts for labeling and basic sentiment analysis.

## 🚧 Current Status

This repo **only covers labeling and analysis**.
Future updates will include:

* Full Urdu dataset creation
* Model training & evaluation pipelines
* More advanced techniques (Deep Learning, Transformers, etc.)

## 🎯 Focus

The project specifically emphasizes **Urdu sentiment analysis**, highlighting the challenges of working with low-resource languages while learning the basics of NLP and ML.


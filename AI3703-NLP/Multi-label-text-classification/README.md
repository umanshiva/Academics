# Text Classification on Research Articles and Domain Texts

This repository contains the implementation for **Assignment 2: Text Classification**, exploring multiple models to predict topics or domains of text data from titles and abstracts.

---

## 📌 Overview
The project applies **machine learning and deep learning models** to classify text into research topics and domains.  
Two datasets were used:
- **Dataset 1:** 20,972 research articles (titles + abstracts) labeled with topics (CS, Physics, Math, Stats, Bio, Finance).  
- **Dataset 2:** 3,927 domain texts labeled as Entertainment, Healthcare, Sports, Technology, or Tourism.

---

## 🛠️ Preprocessing
- Lowercasing, punctuation removal, number removal  
- Tokenization, stopword removal, lemmatization (WordNet)  
- Combined TITLE and ABSTRACT/CONTENT columns into a single text field  
- Represented text with **Word2Vec embeddings (100-dim)**

---

## 🤖 Models Implemented
- **Logistic Regression** – baseline with averaged embeddings  
- **FastText** – efficient text classification with subword support  
- **LSTM** – sequential modeling with Word2Vec initialization  
- **CNN+LSTM** – local feature extraction + sequential dependencies

---

## 📊 Results
| Model           | Dataset 1 F1 | Dataset 2 F1 |
|-----------------|--------------|--------------|
| Logistic Reg.   | 0.38         | 0.82 |
| LSTM            | 0.80         | 0.98 |
| CNN+LSTM        | 0.78         | 1.00 |
| FastText        | 0.76         | 0.89 |

> **Key Insight:** LSTM and CNN+LSTM achieved the highest performance; FastText is a good lightweight alternative.

---

## 🧩 Contributors

- **Umanshiva Ladva**

- **Siddhesh Gholap**

- **Rajiv Chaudhary**

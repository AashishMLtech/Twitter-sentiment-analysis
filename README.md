# 🐦 Twitter Sentiment Analysis using Machine Learning

This project implements **Twitter Sentiment Analysis** with a focus on detecting **hate speech (racism/sexism)** using **Machine Learning algorithms**. It demonstrates how raw tweets can be preprocessed, transformed into numerical features, and classified into **hate** and **non-hate** categories.

The work was carried out as part of a **B.Tech Final Year Project** at **M.J.P. Rohilkhand University, Bareilly**.

---

## 📌 Project Overview
- Title: **Twitter Sentiment Analysis**
- Developer: **Aashish Kumar**  
- Institution: **M.J.P. Rohilkhand University, Bareilly (2025)**  

This project compares **Naïve Bayes, Logistic Regression, and Support Vector Machine (SVM)** for hate speech detection, highlighting strengths and limitations of each model.  

---

## 📊 Dataset
- **Source:** [Kaggle – Twitter Hate Speech Detection Dataset](https://www.kaggle.com/datasets/arkhoshghalb/twitter-sentiment-analysis-hatred-speech/data)  
- **Size:** 6,000 tweets (3,000 hate, 3,000 non-hate after balancing)  
- **Labels:**  
  - `0` → Non-hate (neutral/general tweets)  
  - `1` → Hate speech (racist/sexist tweets)  

---

## 🔎 Data Preprocessing
Steps applied to raw tweets:
1. **Lowercasing** text  
2. **Removing stopwords** (e.g., the, is, are)  
3. **Cleaning tweets** (removing URLs, mentions, hashtags, numbers, punctuation, special characters)  
4. **Stemming & Lemmatization** for standardizing words  
5. **Word Cloud Generation** for visualizing frequent words  

Balanced dataset using **undersampling** → equal hate and non-hate tweets.  

---

## 🛠️ Feature Extraction
- **TF-IDF Vectorization** used to convert tweets into numeric form.  
- Parameters:  
  - Max Features = 5000  
  - N-grams = (1, 2) for unigrams and bigrams  

---

## 🤖 Machine Learning Models
Implemented and evaluated:
1. **Naïve Bayes (NB)**  
   - Simple, fast, but weak in detecting hate speech.  

2. **Logistic Regression (LR)**  
   - Balanced performance, interpretable results.  

3. **Support Vector Machine (SVM)**  
   - Best model for this task, excellent precision and recall.  

### Evaluation Metrics:
- Accuracy  
- Precision  
- Recall  
- F1 Score  
- Confusion Matrix  

---

## 📈 Results
| Model              | Accuracy | Precision (Hate) | Recall (Hate) | F1 (Hate) |
|--------------------|----------|------------------|---------------|-----------|
| Naïve Bayes (NB)   | 94%      | 0.60             | 0.65          | 0.62      |
| Logistic Regression| 96%      | 0.80             | 0.75          | 0.78      |
| **SVM (Best)**     | **98%**  | **0.91**         | **0.89**      | **0.90**  |

**Key Insight:**  
- **SVM outperformed Logistic Regression and Naïve Bayes**.  
- NB struggled with hate speech detection (low recall).  
- SVM achieved the best balance of precision and recall → most suitable for real-world deployment.  

---

## ✅ Conclusion
- Twitter data, though noisy, can be effectively processed for **sentiment and hate speech detection**.  
- **SVM proved most reliable**, achieving **98% accuracy** with high precision and recall.  
- Ethical considerations are critical → false negatives in hate speech detection can worsen online toxicity.  

### 🔮 Future Scope
- Use **Deep Learning & Transformers (BERT, RoBERTa)** for context-aware embeddings.  
- Handle **multilingual & code-mixed tweets**.  
- Expand from binary → **multi-class sentiment analysis**.  
- Deploy real-time **streaming sentiment dashboards**.  

---


---

## ⚙️ Tech Stack
- **Language:** Python  
- **Libraries:** NumPy, Pandas, Matplotlib, Seaborn, NLTK, Scikit-learn  
- **ML Models:** Naïve Bayes, Logistic Regression, Support Vector Machine  

---

## 👨‍💻 Author
**Aashish Kumar**  
B.Tech (Computer Science & Information Technology)  
M.J.P. Rohilkhand University, Bareilly  



---

## 📜 License
This project is for **academic and research purposes only**.  
Please provide citation if reused.  

---


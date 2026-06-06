#  Sentiment Analysis of IMDB Movie Reviews

---

##  Problem Statement
Predict whether a movie review is **positive** or **negative** using Natural Language Processing and Machine Learning techniques — and compare multiple models to find the best approach.

---

## 📂 Dataset
| Property | Details |
|----------|---------|
| Name | IMDB Dataset of 50K Movie Reviews |
| Source | [Kaggle](https://www.kaggle.com/code/lakshmi25npathi/sentiment-analysis-of-imdb-movie-reviews/input) |
| Size | ~66 MB |
| Reviews | 50,000 (25,000 positive, 25,000 negative) |
| Balance | Perfectly balanced dataset |
| Split | 40,000 train / 10,000 test (stratified) |

---

## 🤖 Models Used
- Logistic Regression *(original + tuned with GridSearchCV)*
- SVM — SGD Classifier *(original)*
- Multinomial Naive Bayes *(original)*
- **Random Forest** *(new — extension)*

---

## 📊 Key Results

| Model | Accuracy | F1 Score | Precision | Recall |
|-------|----------|----------|-----------|--------|
| Logistic Regression (BoW) | 0.75 | 0.75 | 0.75 | 0.76 |
| Logistic Regression (TF-IDF) | 0.75 | 0.75 | 0.75 | 0.75 |

> Results evaluated on 10,000 test samples (4,993 Positive / 5,007 Negative).

---

##  Preprocessing Pipeline
1. HTML tag removal
2. Square bracket noise removal
3. **Emoji removal** *(extension)*
4. **Negation handling** *(extension)*
5. Special character removal
6. Stopword removal *(preserving negation words)*
7. Lowercasing


---

##  Libraries Used
```
numpy | pandas | scikit-learn | nltk | matplotlib
seaborn | wordcloud | beautifulsoup4 | textblob | spacy
```

---

##  Repository Structure
```
sentiment-analysis/
│
├── sentiment-analysis-extended.ipynb   # Main extended notebook
└── README.md                           # Project documentation
```





## 🙏 Acknowledgement
Original notebook by [Lakshmi Narayana](https://www.kaggle.com/code/lakshmi25npathi/sentiment-analysis-of-imdb-movie-reviews) on Kaggle. This work extends it with additional preprocessing, models, tuning, and evaluation components.

# Sentiment Analysis on Customer Reviews

## Project Overview
This project implements an **end-to-end sentiment analysis system** to classify customer reviews into **positive** and **negative** sentiments. The objective is to automatically analyze customer feedback and help businesses understand customer satisfaction and complaints at scale.

---

## Dataset
- Customer review text data
- Imbalanced dataset with a higher number of positive reviews
- Sentiment labels were derived from rating values

---

## Exploratory Data Analysis (EDA)
- Analyzed class distribution to understand data imbalance
- Performed word frequency analysis for positive and negative reviews
- Word clouds were used **only for exploratory understanding**, not for model training

---

## Text Preprocessing
The following preprocessing steps were applied:
- Converted text to lowercase
- Removed punctuation and numbers
- Removed stopwords
- Cleaned extra spaces

---

## Feature Engineering
- Used **TF-IDF Vectorization** to convert text data into numerical features
- This helped capture important words while reducing the impact of commonly occurring terms

---

## Models Used
The following machine learning models were trained and compared:
1. **Logistic Regression**
2. **Naive Bayes (MultinomialNB)**

---

## Model Evaluation
Models were evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

### Model Performance
| Model | Accuracy |
|------|----------|
| Logistic Regression | 98.77% |
| Naive Bayes | 98.77% |

Although both models achieved similar accuracy, **Naive Bayes was selected as the final model** due to its simplicity, probabilistic nature, and suitability for large-scale text classification tasks.

---

## Key Results
- High recall for negative reviews ensured that critical customer complaints were not missed
- The model generalized well on unseen test data
- Naive Bayes provided a strong and efficient baseline for sentiment classification

---

## Business Use Case
This sentiment analysis system can be used to:
- Automatically monitor customer feedback
- Identify negative reviews and complaints
- Improve product quality and customer experience
- Enable data-driven decision making

---

## 🛠️ Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
- NLTK
- Matplotlib

## Conclusion
TF-IDF combined with Naive Bayes proved to be highly effective for sentiment classification on customer review data. The model achieved strong and consistent performance across all evaluation metrics and can be reliably used for real-world customer feedback analysis.

---

## Future Improvements
- Handle neutral sentiment as a separate class
- Experiment with deep learning models such as LSTM or BERT
- Deploy the model using Flask or FastAPI

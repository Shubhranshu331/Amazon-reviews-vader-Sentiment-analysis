# Sentiment Analysis on Amazon Fine Food Reviews

This project performs sentiment analysis on the Amazon Fine Food Reviews dataset using the VADER (Valence Aware Dictionary and sEntiment Reasoner) model from NLTK. The goal is to analyze how textual sentiment aligns with user-provided star ratings.

---

## 📊 Dataset

- **Source**: Amazon Fine Food Reviews (Kaggle): [https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews](https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews)
- Contains user reviews including:
  - Review text
  - Summary
  - Star ratings (1–5)
  - User and product metadata

A subset of 20,000 reviews is used for efficient analysis.

---

## ⚙️ Approach

### 1. Data Loading
- Dataset is loaded using Pandas
- Limited to first 20,000 entries for faster processing

### 2. Exploratory Data Analysis (EDA)
- Distribution of review scores (1–5 stars)
- Visualization of rating frequency

### 3. Text Processing (NLTK)
- Tokenization
- Part-of-speech tagging
- Named entity recognition (demonstration)

### 4. Sentiment Analysis (VADER)
- Each review is analyzed using VADER
- Generates sentiment scores:
  - Positive (`pos`)
  - Neutral (`neu`)
  - Negative (`neg`)
  - Compound score (`compound`)

### 5. Data Integration
- Sentiment scores are merged with original dataset
- Enables comparison between text sentiment and ratings

### 6. Visualization
- Compound sentiment score vs star ratings
- Breakdown of positive, neutral, and negative scores across ratings

---

## 📈 Results

- Higher star ratings generally correspond to higher positive sentiment scores
- Lower ratings show increased negative sentiment
- Neutral sentiment is distributed across all rating levels

These trends indicate that VADER captures overall sentiment patterns in user reviews effectively.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- NLTK (VADER Sentiment Analyzer)

---

## ⚠️ Limitations

- VADER is a lexicon-based model and may not fully capture:
  - Sarcasm
  - Contextual nuances
  - Domain-specific language
- No supervised learning or model training is performed

---

## 🚀 Future Scope

- Apply machine learning or deep learning models for improved accuracy
- Perform sentiment classification and evaluation
- Extend analysis to full dataset

---

## 📌 Conclusion

This project demonstrates how lexicon-based sentiment analysis can be applied to real-world review data to extract meaningful insights and observe patterns between textual sentiment and user ratings.

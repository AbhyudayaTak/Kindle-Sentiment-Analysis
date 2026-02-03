# Kindle Sentiment Analysis

## Overview
This project performs sentiment analysis on Amazon Kindle Store book reviews using machine learning and natural language processing (NLP) techniques. The goal is to classify reviews as positive or negative based on their textual content, demonstrating end-to-end data science skills from data preprocessing to model evaluation.

## Dataset
- **Source:** Amazon Kindle Store 5-core dataset (May 1996 - July 2014)
- **Size:** 982,619 reviews
- **Features:**
  - `asin`: Product ID
  - `helpful`: Helpfulness rating
  - `overall`: Product rating
  - `reviewText`: Review text
  - `reviewTime`: Review date
  - `reviewerID`: Reviewer ID
  - `reviewerName`: Reviewer name
  - `summary`: Review summary
  - `unixReviewTime`: Unix timestamp

## Key Steps & Techniques
1. **Data Loading & Exploration**
   - Loaded reviews from CSV
   - Explored data structure, missing values, and class distribution
2. **Data Preprocessing**
   - Lowercased text
   - Removed special characters, stopwords, URLs, and HTML tags
   - Lemmatized words for normalization
   - Converted ratings to binary sentiment (positive/negative)
3. **Feature Engineering**
   - Bag-of-Words (BoW) and TF-IDF vectorization
4. **Modeling**
   - Trained Naive Bayes classifiers on BoW and TF-IDF features
   - Evaluated using accuracy, confusion matrix, and classification report

## Results
- Achieved robust sentiment classification using both BoW and TF-IDF features
- **Bag-of-Words (BoW) Accuracy:** 57.75%
- **TF-IDF Accuracy:** 57.21%
- Demonstrated the impact of text preprocessing and feature engineering on model performance

## Skills Demonstrated
- Data wrangling and cleaning (pandas, regex, BeautifulSoup)
- NLP preprocessing (NLTK, lemmatization, stopword removal)
- Feature extraction (CountVectorizer, TfidfVectorizer)
- Machine learning (scikit-learn, Naive Bayes)
- Model evaluation and interpretation

## How to Run
1. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
2. **Run the notebook:**
   Open `kindlesentiment.ipynb` in VS Code or Jupyter and execute cells sequentially.

## Why This Project Stands Out
- **End-to-End Pipeline:** Covers the full data science workflow from raw data to model evaluation
- **Real-World Dataset:** Uses a large, authentic dataset with practical business relevance
- **Clean, Modular Code:** Follows best practices for readability and reproducibility
- **Resume Impact:** Demonstrates hands-on experience with NLP, feature engineering, and ML modeling

## Potential Extensions
- Hyperparameter tuning and advanced models (SVM, XGBoost)
- Deep learning approaches (LSTM, BERT)
- Sentiment visualization and dashboarding
- Fake review detection and product recommendation

## References
- [Amazon Product Data (Julian McAuley, UCSD)](http://jmcauley.ucsd.edu/data/amazon/)

---
**Author:** Abhyudaya Tak


# Sentiment Analysis Project

## Description
This project performs sentiment analysis on user reviews from the Google Play Store. The workflow includes data scraping, preprocessing, visualization, and model training using both Machine Learning and Deep Learning techniques.

## Features
- **Data Scraping:** Extracts reviews using `google_play_scraper`.
- **Data Preprocessing:** Cleans text, removes duplicates, and applies tokenization, stopword removal, and stemming.
- **Visualization:** Generates word clouds and plots review distributions.
- **Machine Learning Models:** Logistic Regression, Random Forest, SVM.
- **Deep Learning Models:** LSTM and BiLSTM.
- **Performance Evaluation:** Compares accuracy across models and feature extraction techniques (TF-IDF, CountVectorizer).

## Dependencies
Ensure the following Python libraries are installed:
```bash
pip install google_play_scraper pandas numpy nltk seaborn wordcloud sklearn imblearn keras tensorflow
```

## How to Run
1. Clone this repository

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebooks in sequence:
   - `scraping.ipynb` (Extracts data from Google Play Store)
   - `notebook.ipynb` (Preprocessing, visualization, and model training)

## Results
- The dataset contains **13,379 samples** across three sentiment classes.
- **BiLSTM** achieved the highest accuracy (**97.31%**).
- Using **SMOTE** sampling improved the performance of Machine Learning models.
- **SVM with CountVectorizer and SMOTE** is recommended for faster training with competitive accuracy.

## Recommendations
1. Use **BiLSTM** for best accuracy.
2. If computational resources are limited, **SVM with CountVectorizer** is a good alternative.
3. Further tuning on data balancing and feature extraction may enhance results.
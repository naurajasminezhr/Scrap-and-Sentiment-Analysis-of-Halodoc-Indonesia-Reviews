# Scrap-and-Sentiment-Analysis-of-Halodoc-Indonesia-Reviews
This project involves scraping and analyzing Halodoc app reviews from Google Play Store. It includes web scraping, data preprocessing (language detection, text cleaning, stemming), and sentiment analysis. The analysis provides insights into user sentiment, frequent words in reviews, and the relationship between ratings and sentiment scores.

# Scraping and Sentiment Analysis of Halodoc Reviews

This repository contains a comprehensive analysis of Halodoc app reviews, including web scraping, data preprocessing, and sentiment analysis. The project aims to extract insights from user reviews to understand the overall sentiment and key topics discussed by users of the Halodoc healthcare platform.

## Overview

This project involves several key steps:
1. Web scraping to collect Halodoc app reviews from the Google Play Store
2. Data preprocessing, including language detection, text cleaning, and stemming
3. Sentiment analysis to determine the polarity of reviews
4. Visualization of results, including word clouds and scatter plots

## Prerequisites

- Python 3.x
- Libraries: pandas, numpy, matplotlib, seaborn, nltk, Sastrawi, langdetect, textblob, wordcloud

## Installation

To set up the environment, follow these steps:

1. Clone the repository:
```
   https://github.com/naurajasminezhr/Scrap-and-Sentiment-Analysis-of-Halodoc-Indonesia-Reviews.git
```

2. Navigate to the repository:
```
cd Scrap-and-Sentiment-Analysis-of-Halodoc-Indonesia-Reviews
```
3. Install required libraries:
```
pip install -r requirements.txt
```
## Project Structure
```
halodoc-review-analysis/
├── data/
│ ├── raw/
│ │ └── df_halodoc.csv
│ └── processed/
│ ├── df_halodoc_after_detectlang.csv
│ ├── df_halodoc_after_sentiment_rating.csv
│ ├── df_halodoc_after_stemming.csv
│ └── df_halodoc_before_stopwords_sentiment_rating.csv
├── notebooks/
│ └── Scrap_and_Sentiment_Analysis_Halodoc_Reviews_5026211005_pba_indoreviews.ipynb
├── results/
│ ├── scatterplot_GooglePlayStore_HaloDoc_Reviews_SentimentAnalysis.png
│ ├── freqwords_before_stopwords_HaloDoc_Reviews.png
│ ├── wordclouds_before_stopwords_HaloDoc_Reviews.png
│ ├── stemmer_wordclouds_HaloDoc_Reviews.png
│ ├── rating_score_HaloDoc_Reviews.png
│ └── frequency_words_HaloDoc.png
├── README.md
└── requirements.txt
```

## Functions

The Jupyter notebook includes the following main functions:

1. **Web Scraping**: Scraping Halodoc app reviews from the Google Play Store.
2. **Data Preprocessing**: 
   - Language detection
   - Text cleaning (removing special characters, converting to lowercase)
   - Stopword removal
   - Stemming using Sastrawi stemmer
3. **Sentiment Analysis**: Using TextBlob to determine sentiment polarity and subjectivity.
4. **Visualization**: 
   - Word clouds for frequent words
   - Scatter plots for sentiment analysis
   - Bar plots for rating distribution

## Libraries

- pandas: Data manipulation and analysis
- numpy: Numerical computing
- matplotlib & seaborn: Data visualization
- nltk: Natural Language Processing tasks
- Sastrawi: Indonesian language stemming
- langdetect: Language detection
- textblob: Sentiment analysis
- wordcloud: Word cloud generation

## Getting Started

1. Open the Jupyter Notebook:
```
jupyter notebook Scrap_and_Sentiment_Analysis_Halodoc_Reviews_5026211005_pba_indoreviews.ipynb
```

2. Run the notebook cells sequentially to perform the analysis.

## Results

The analysis of Halodoc app reviews provided several quantitative insights:

1. Data Volume:
   - Total reviews analyzed: 35,931

2. Language Distribution:
   - Reviews in English: 20,113 (56.0%)
   - Reviews in Indonesian: 15,818 (44.0%)

3. Sentiment Distribution:
   - Positive reviews: 31,911 (88.8%)
   - Negative reviews: 3,265 (9.1%)
   - Neutral reviews: 755 (2.1%)

4. Rating Distribution:
   - 5-star ratings: 29,710 (82.7%)
   - 4-star ratings: 2,201 (6.1%)
   - 3-star ratings: 755 (2.1%)
   - 2-star ratings: 601 (1.7%)
   - 1-star ratings: 2,664 (7.4%)

5. Most Frequent Words (after stemming):
   - Top 5 words: "bantu" (8,166), "good" (4,380), "kasih" (3,171), "terima" (3,080), "helpful" (2,545)

6. Key Visualizations:
   - Word clouds highlighting frequent terms in reviews
   - Scatter plot showing the relationship between sentiment polarity and subjectivity
   - Bar plot of rating distribution
   - Frequency distribution of top words before and after stemming


## Evaluation

The project doesn't include a formal evaluation metric, as it's primarily an exploratory analysis. However, the effectiveness of the sentiment analysis can be assessed by comparing the calculated sentiment scores with the actual review ratings.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

The MIT License is a permissive free software license originating at the Massachusetts Institute of Technology (MIT). It puts only very limited restriction on reuse and has, therefore, high license compatibility.

Key points of the MIT License:
- It allows users to do anything with the code, including using it commercially.
- The only requirement is that the license and copyright notice must be included with the code.
- It provides no warranty or liability protection for the original author.

For the full license text, please refer to the LICENSE file in this repository.

## Acknowledgments

- Google Play Store for providing the review data
- Halodoc users for their valuable feedback

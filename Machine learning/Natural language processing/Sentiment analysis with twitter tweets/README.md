# Sentiment Analysis on Electricity Tweets in India and UK  

## Project Overview

This project performs sentiment analysis on tweets related to electricity in India and the UK. By analyzing public sentiment towards electricity-related topics, the project provides insights that can aid policymakers, businesses, and researchers in understanding public opinions and trends. The analysis involves data collection, preprocessing, sentiment classification, and model evaluation.

## Key Components

1. **Data Collection**
   - Tweets are collected using the Twitter API with the Tweepy library.
   - Tweets are fetched based on specific hashtags and geolocations for India and the UK.

2. **Data Preprocessing**
   - **Removing Patterns:** Strips out unwanted patterns such as mentions, retweets, and other irrelevant text.
   - **Filtering Links:** Removes words containing links.
   - **Removing Duplicates:** Eliminates duplicate tweets to ensure unique entries.
   - **Cleaning Text:** Removes punctuation, numbers, and special characters; filters out common stopwords.
   - **Tokenization and Lemmatization:** Splits the text into tokens, lemmatizes words to their base forms, and reassembles the tokens into cleaned sentences.

3. **Sentiment Analysis**
   - Utilizes the VADER sentiment analyzer from the NLTK library to classify tweets as positive or negative.
   - Adds sentiment labels to the tweets, providing insights into public sentiment.

4. **Model Training and Evaluation**
   - Trains and evaluates several machine learning models, including Decision Tree, Random Forest, Logistic Regression, and Naive Bayes.
   - Compares model performance based on metrics such as accuracy and F1 score to identify the most effective model for sentiment classification.

## Requirements

Ensure you have the following Python libraries installed:

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `re`
- `time`
- `string`
- `warnings`
- `nltk`
- `wordcloud`
- `scikit-learn`
- `tweepy`
- `textblob`
- `tensorflow`
- `keras`

Install these libraries using pip:

```bash
pip install numpy pandas matplotlib seaborn nltk wordcloud scikit-learn tweepy textblob tensorflow keras
```

## Setup

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/your-repository.git
   cd your-repository
   ```

2. **Download NLTK Data:**

   Run the following commands in a Python environment to download required NLTK datasets:

   ```python
   import nltk
   nltk.download('stopwords')
   nltk.download('wordnet')
   nltk.download('vader_lexicon')
   nltk.download('averaged_perceptron_tagger')
   nltk.download('movie_reviews')
   nltk.download('punkt')
   nltk.download('conll2000')
   nltk.download('brown')
   ```

3. **Twitter API Credentials:**

   Replace the placeholders in your script with your Twitter API credentials:

   ```python
   consumer_key = 'YOUR_CONSUMER_KEY'
   consumer_secret = 'YOUR_CONSUMER_SECRET'
   access_token = 'YOUR_ACCESS_TOKEN'
   access_token_secret = 'YOUR_ACCESS_TOKEN_SECRET'
   ```

## Usage

1. **Data Collection:**
   - Use the `Tweets_extractor` function to fetch tweets based on hashtags and geolocations.

2. **Data Preprocessing:**
   - Apply the `data_preprocessing` method from the `Preprocessing` class to clean the collected tweets.

3. **Sentiment Analysis:**
   - Utilize the `Sentiment_analysis` class to perform sentiment classification on the cleaned tweets.

4. **Model Training:**
   - Train and evaluate machine learning models to determine the best algorithm for sentiment analysis.

## Results

- The project provides a detailed analysis of sentiment trends in electricity-related tweets.
- Model performance is compared to identify the most accurate sentiment classifier.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Thanks to the developers of the Tweepy, NLTK, TextBlob, and scikit-learn libraries.
- Special thanks to the contributors of the open-source tools used in this project.

## Contact

For any questions or feedback, please contact me at ( Check my github profile contact section ).

# SentimentSniffer

Overview
SentimentSniffer is a Python project designed to perform sentiment analysis on text data, particularly tweets. It utilizes Natural Language Processing (NLP) techniques along with machine learning models to classify the sentiment of tweets into three categories: positive, negative, and neutral.

Libraries Required
The following libraries are required to run the SentimentSniffer project:

Pandas: For data manipulation and analysis.
NumPy: For numerical computations.
Regular Expressions (re): For text cleaning.
spaCy: For NLP-related tasks such as tokenization and lemmatization.
scikit-learn: For machine learning models and evaluation metrics.


sentiment_analyzer(tweet)
The sentiment_analyzer(tweet) function is the core of the SentimentSniffer project. Given a tweet as input, it performs the following steps:

1.Text Cleaning:
Removes user mentions, links, and special characters.
Converts text to lowercase.
Lemmatizes the text to reduce words to their base form.

2.Feature Engineering:
Uses TF-IDF (Term Frequency-Inverse Document Frequency) to convert the cleaned tweet into numerical features.

3.Sentiment Prediction:
Utilizes the trained Logistic Regression model to predict the sentiment of the tweet.
Returns the predicted sentiment label ('positive', 'negative', or 'neutral').


Example Usage

# Importing required libraries
import SentimentSniffer

# Example tweet
tweet = "@USAirways flt 419. 2+ hrs Late Flight, baggage + 1 more hr. Now I see they delivered my suitcase wet inside &amp; out. #NotHappy"

# Analyzing sentiment
predicted_sentiment = SentimentSniffer.sentiment_analyzer(tweet)
print("Predicted Sentiment:", predicted_sentiment)

Output:
Predicted Sentiment: ['negative']
Conclusion
SentimentSniffer provides a simple yet effective solution for sentiment analysis of tweets. By leveraging NLP techniques and machine learning models, it accurately predicts the sentiment of text data, which can be valuable for various applications such as social media monitoring, customer feedback analysis, and brand sentiment analysis.

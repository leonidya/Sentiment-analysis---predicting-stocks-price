## Research Question: "Can sentiment analysis of financial text data provide insight and predict increase or decrease of stock's price?" (Sentiment Analysis for Financial Data) 

Predicting decrease or increase in stock's price based on tweets sentiment analysis
In this project I'm going to train sentiment analysis models - in order to analyse the
sentiment of financial data (tweets). Social media, news and professional opinion (financial analyst opinions) tend to inflect
greatly on stocks prices, it's enogh for Elon Musk to tweet : "Twitter deal temporarily on
hold", for the stock of Twitter to drop by 18%. While there are many pre-trained sentiment analysis models, and much data along the
interent to train your own sentiment analysis model - the main goal of our research is to train dedicated sentiment analysis model to deal with financial data.
The agenda is that a dedicated model, adjusted to the specific type of data you want to work with, even if it's small - will deal better with the task, than a more large but generic model. In this project I will train dedicated sentiment analysis model for financial data. In addition, I'll
compare it's performance with models trained on generic data, make predictions and evaluate them, and finally make conclusions.

### About the Data:

Training Data:

1. Stock Market Tweet | Sentiment Analysis lexicon
https://www.kaggle.com/datasets/utkarshxy/stock-markettweets-lexicon-data
(https://www.kaggle.com/datasets/utkarshxy/stock-markettweets-lexicon-data)
Tweets were collectect between April 9 and July 16, 2020 using SPX500 and the top 25
companies in the index and "#stocks". 1300 tweets were manually classified and
reviewed. contains the following columns:
- ID -> Contains id used for the tweet.
- Tweet -> Tweet/text written by the user.
- Sentiment -> Wheter the tweet was postive, neutral or negative.

2. Stock-Market Sentiment Dataset
https://www.kaggle.com/datasets/yash612/stockmarket-sentiment-dataset
(https://www.kaggle.com/datasets/yash612/stockmarket-sentiment-dataset)
a dataset created by YASH CHAUDHARY, and shared on Kaggle.
Data description: manually labeled tweets of financial data. There is no date regarding
the tweets - last update was in 2020 - 3 years ago. contains around 5.7K labeled tweets
(2.1K negative and 3.6K positive). contains the following columns:
- Text -> Tweet text
- Sentiment -> positive (1) negative (-1)

3. FinancialPhraseBank
https://metatext.io/datasets/financialphrasebank
(https://metatext.io/datasets/financialphrasebank)
a dataset created by Malo et al. in 2014. and shared by ANKUR SINHA in Kaggle.
Data description: FinancialPhraseBank data, contains the sentiments for financial news
headlines from the perspective of a retail investor. contains around 4.8K sentences.
contains the following columns:
- News Headline -> News Headline.
- Sentiment -> Wheter the tweet was positive, neutral or negative.

4. Stock News Sentiment Analysis
https://www.kaggle.com/datasets/avisheksood/stock-news-sentiment-analysismassive-dataset
(https://www.kaggle.com/datasets/avisheksood/stock-news-sentiment-analysismassive-dataset)
a dataset created by AVISHEK AVISHEK, and shared on Kaggle. mannualy created by the
author, covers chosen sentences from news from february 2003 till august 2022.
contains arond 108K sentences and labels, unfortunatelly after manual review of the data
only the first 8.2K rows were found usefull. contains the following columns:
- Sentence -> sentence from news.
- Sentiment -> positive (1) neutral or negative (0).

5. Auditor sentiment dataset
https://huggingface.co/datasets/FinanceInc/auditor_sentiment/blob/main/README.md
(https://huggingface.co/datasets/FinanceInc/auditor_sentiment/blob/main/README.md)
Data description: Auditor sentiment dataset of sentences from financial news. The
dataset consists of several thousand sentences from English language financial news
categorized by sentiment. split into train and test data, will be used as trained data only -
total of 4840 sentences. contains the following columns:
- sentence: a tokenized line from the dataset
- label: a label corresponding to the class as a string: 'positive' - (2), 'neutral' - (1), or
'negative' - (0)
Total Training data ~ 25K short text (7K tweets, 4.8K News Headlines, 13K news sentences)

### Test Data - Unlabeled

1. Stock Tweets for Sentiment Analysis and Prediction
https://www.kaggle.com/datasets/equinxx/stock-tweets-for-sentiment-analysis-and-prediction
(https://www.kaggle.com/datasets/equinxx/stock-tweets-for-sentiment-analysis-and-prediction)
A dataset created by HANNA YUKHYMENKO, and shared on Kaggle.
Data description: The dataset contains about 80K tweets for top 25 most watched stock
tickers on Yahoo Finance from 30-09-2021 to 30-09-2022. contains the following
collumns:
• Date - date and time of tweet
• Tweet - full text of the tweet
• Stock Name - full stock ticker name for which the tweet was scraped
• Company Name - full company name for corresponding tweet and stock ticker
This data is unlabeled, so the evaluation of the predictions will be according to the real stock's
prices on Yahoo finance.
Total test data ~ 80K tweets

Still in progress...

## Research Question: "Can sentiment analysis of financial text data provide insight and predict increase or decrease of stock's price?" (Sentiment Analysis for Financial Data) 

![image](https://user-images.githubusercontent.com/53173112/226352464-112a1272-7d59-4310-912c-8021a43a2a9d.png)

Predicting decrease or increase in stock's price based on tweets sentiment analysis
In this project I'm going to train sentiment analysis models - in order to analyse the
sentiment of financial data (tweets). Social media, news and professional opinion (financial analyst opinions) tend to inflect
greatly on stocks prices, it's enogh for Elon Musk to tweet : "Twitter deal temporarily on
hold", for the stock of Twitter to drop by 18%. While there are many pre-trained sentiment analysis models, and much data along the
interent to train your own sentiment analysis model - the main goal of our research is to train dedicated sentiment analysis model to deal with financial data.
The agenda is that a dedicated model, adjusted to the specific type of data you want to work with, even if it's small - will deal better with the task, than a more large but generic model. In this project I will train dedicated sentiment analysis model for financial data. In addition, I'll
compare it's performance with models trained on generic data, make predictions and evaluate them, and finally make conclusions.

![image](https://user-images.githubusercontent.com/53173112/226362166-c60eeaa9-7a1f-4f3f-9ea0-69dbf2b266fc.png)


![image](https://user-images.githubusercontent.com/53173112/226354767-7b55e4bc-ab59-4956-812f-ba517a5104ef.png)

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

### Some Insigths

![image](https://user-images.githubusercontent.com/53173112/226354977-37ad5055-daa5-4b52-81c1-ffd8600125be.png)

![image](https://user-images.githubusercontent.com/53173112/226355149-da8aaf86-7936-4b4e-9635-47b3075bb222.png)

![image](https://user-images.githubusercontent.com/53173112/226355207-38e802e4-35e6-49da-aca1-6742eb708c58.png)

![image](https://user-images.githubusercontent.com/53173112/226355295-764e7af4-de6e-4f14-862e-110cf1488235.png)

![image](https://user-images.githubusercontent.com/53173112/226355342-c30d592b-d179-4a6e-99b2-ccde0bd6190f.png)

![image](https://user-images.githubusercontent.com/53173112/226355380-f0f200e5-5aae-4562-ac76-e512ca614fa5.png)

![image](https://user-images.githubusercontent.com/53173112/226355433-c4440889-4ac5-4075-a8db-eccf49fc2485.png)

![image](https://user-images.githubusercontent.com/53173112/226355511-52a3141d-304b-4104-88ec-0f10fe4e463d.png)

![image](https://user-images.githubusercontent.com/53173112/226355548-87ac4862-0d8b-4c2d-881f-3f187c383b53.png)

![image](https://user-images.githubusercontent.com/53173112/226355585-0abcb417-bfe8-42ef-9c4a-8db2723e061f.png)


RESULTS:

![image](https://user-images.githubusercontent.com/53173112/226355667-cf334091-69db-4368-b196-1f36a3c5c787.png)

![image](https://user-images.githubusercontent.com/53173112/226355741-a1a1720a-cc02-4a38-8c7b-4b075029de5c.png)

![image](https://user-images.githubusercontent.com/53173112/226355794-49965dec-62b3-47ad-a6ba-e6f9c6b3ae37.png)

![image](https://user-images.githubusercontent.com/53173112/226355896-a76d124c-0437-4c0a-80ef-743a584daf90.png)

![image](https://user-images.githubusercontent.com/53173112/226355943-7f521c3c-ea90-4c85-9f1d-46bb0764b4e9.png)

![image](https://user-images.githubusercontent.com/53173112/226355998-79e86f00-4f40-4b9d-a506-2ee059efd997.png)

![image](https://user-images.githubusercontent.com/53173112/226354160-884eb684-e0ba-40bf-a6cb-966ee75ecf88.png)

I began by exploring whether sensitivity analysis has an impact on the stock price. I was aware beforehand that due to technical limitations and data constraints, it was unlikely that I would be able to draw definitive conclusions. Achieving such conclusions would have likely resulted in significant financial gain. However, I acknowledge that the information gathered can still be useful. My research serves as a foundation for future studies that can yield more conclusive findings. The main objective is to continue building upon my work to reach definitive outcomes in the future.

Findings have revealed that sensitivity analysis can provide valuable insights into the emotional and quantitative reactions of individuals throughout the week, which can be utilized by businesses to their advantage. For instance, companies can strategically time the release of their negative reports on Monday when there is heightened activity, and release positive news during the middle of the week. In the event of a significant management change, such as the resignation of a CEO, it is recommended that the company announce it on a Monday.

Furthermore, for financial analysts, it is advisable to refrain from publishing reports on Mondays, or at the very least, consider the optimistic sentiment that typically characterizes this day of the week. Waiting until the middle of the week may provide a more accurate picture of the company's situation, as there may be additional news or events that could impact the market sentiment. 

Moreover, we can see the significance of effective foreign relations management for companies. My findings indicate that even when a company's share price experiences a sustained decline, positive reactions on social media platforms can offset the negative impact (Tesla -  Elon Musk). This suggests that companies that invest in enhancing their foreign relations, through effective leadership or other channels, can maintain a positive reputation, despite fluctuations in the stock market.

Overall, research demonstrates the practical applications of sensitivity analysis, and the potential benefits it can offer to various stakeholders in the business world.


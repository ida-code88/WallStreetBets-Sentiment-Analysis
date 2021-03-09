# WallStreetBets-Sentiment-Analysis For Beginner

r/wallstreetbets, also known as WallStreetBets or WSB, is a subreddit where participants discuss stock and option trading. It has become notable for its profane nature, aggressive trading strategies, and role in the GameStop short squeeze that caused losses on short positions in U.S. firms topping US$70 billion in a few days in early 2021. The subreddit is famous for its colorful jargon and terms.[1]

As this post is for ones who new to sentiment analysis algorithm, what we will do is quite simple. Start from analysing posts from r/wallstreetbets users or people who interest with the topic. 

The dataset is obtained from https://www.kaggle.com/gpreda/reddit-wallstreetsbets-posts 

## Libraries
* Panda
* Numpy
* Matplotlib
* nltk
* wordcloud

## Methods
### Data Processing
* We want to know trend of reddit post within a week. 
  By plotting number of post and day they were posted, we will know the most active-day on reddit forum. We do that by aggregating timestamp into date and day of the week (day name).

### Get Sentiment Value for title and body post
  We do that by separating title and body column into their own dataframe, drop na, do stemming, clean the text, obtain the sentiment values using nltk SentimentIntensityAnalyzer, and then we plot them.
  
### Generate Wordlouds
We generate wordclouds for both title and body, also wordclouds for each sentiment (negative, positive, and neutral). Detail can be seen in the code ipynb file.


[1] https://en.wikipedia.org/wiki/R/wallstreetbets

References:

https://www.kaggle.com/melvinlinus/sentimental-analysis-of-r-wallstreetbets-posts

https://www.kaggle.com/sprakshith/beginner-s-guide-to-sentiment-analysis

https://www.kaggle.com/andreshg/nlp-natural-languague-processing-guidelines

https://www.kaggle.com/radema/yolo-explorative-analysis-on-wallstreetbets

https://www.kaggle.com/thomaskonstantin/reddit-wallstreetbets-posts-sentiment-analysis

# Project2

## Phase 1 
Twitter.py is a program that search twitters using a keyword fiter from the current stream. It displays 50 tweets from the specific user that you are searching(searching can also be changed in the function). The search result basically contains every contend of tweets(eg: @, user name, links...). In phase 2, this unrelated contends shall be removed.

Also, due to restriction of access, this program can only read from the stream. In higer-level permission, the Twitter-API actually will enable writing and performing changes in twitter account.

The resources used for Twitter-API is listed below:
#https://realpython.com/twitter-bot-python-tweepy/

Crendantials:# Authenticate to Twitter

auth = tweepy.OAuthHandler("CONSUMER_KEY", "CONSUMER_SECRET")
auth.set_access_token("ACCESS_TOKEN", "ACCESS_TOKEN_SECRET")


Tesing result:<img width="664" alt="Screen Shot 2020-10-04 at 22 31 23" src="https://user-images.githubusercontent.com/52185318/95036582-61c39200-0696-11eb-96d9-1617f5609b8c.png">

#GOOGLE Natural language processing implementation.
1. create credentials 

https://cloud.google.com/natural-language/automl/docs/quickstart?authuser=2

In terminal, run: export GOOGLE_APPLICATION_CREDENTIALS="/home/user/Downloads/my-key.json"
The google Natural language processing documentations can be found at:
https://cloud.google.com/natural-language/docs/setup

In this project, I specifically implemented a sentiment analysis code to test the polarity in a sentence.

<img width="731" alt="Screen Shot 2020-10-05 at 11 23 09" src="https://user-images.githubusercontent.com/52185318/95099123-84d55c80-06fd-11eb-9190-f01a25308da5.png">

## phase2
This is a program that integrate Twitter API with Google NLP API. It is used to search twitter by keywords among a entire day period. Some search stradigies are used to simplfy the whole process. For example, in this program, a function is used to get rid of symbols like "@" or numbers or hyperlinks which make no sense in NLP system, also, all the textes are converted to lower case to avoid missunderstanding. The pro-processed words will then be sent into Google NLP to do sentiment analysis. In this sample, the program will do 50 tweets at one iteration, so the final result would be an average sentiment. 

### User Story: product manager could simply use this API to keep track of market reaction and use the data to analyse the estimated sale amount. Also, the film company could gather trend topics by using this API to do more movies.



### MVP: I would say the MVP would be Twitter's cooperation, because twitter is a huge platform that we could get data from the whole world. Information there are comprehensive and also it reflects the current trends. As a result, the API analysis would only make sense if we could get as big data flow as we want to do an relatively unbiased language processing.


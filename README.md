# Project2

Phase 1
Twitter.py is a program that search twitters using a keyword fiter from the current stream. It displays 50 tweets from the specific user that you are searching(searching can also be changed in the function). The search result basically contains every contend of tweets(eg: @, user name, links...). In phase 2, this unrelated contends shall be removed.

Also, due to restriction of access, this program can only read from the stream. In higer-level permission, the Twitter-API actually will enable writing and performing changes in twitter account.

The resources used for Twitter-API is listed below:
#https://realpython.com/twitter-bot-python-tweepy/

Crendantials:# Authenticate to Twitter

auth = tweepy.OAuthHandler("CONSUMER_KEY", "CONSUMER_SECRET")
auth.set_access_token("ACCESS_TOKEN", "ACCESS_TOKEN_SECRET")


Tesing result:


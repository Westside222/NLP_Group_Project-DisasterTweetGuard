# NLP_Group_Project-DisasterTweetGuard
--------------------------------------------------------------------------------------------------------------------------
# Context

You are working for a news agency that aims to bring the information on disasters to public attention as soon as possible.

To source the news your department relies on scraping twitter posts algorithmically.

A simple approach is to detect key words that may suggest a disaster.

But this approach can have many false positives. For example, the post: “The crowd was on fire at the concert last night!” does not imply a real disaster.

So detection of words/phrases that may indicate disasters is not sufficient.

The entire context of the tweets needs to be processed to classify the tweet into (1) Disaster or (2) No Disaster

--------------------------------------------------------------------------------------------------------------------------
Train and test data need to be download from https://www.kaggle.com/competitions/nlp-getting-started/data
--------------------------------------------------------------------------------------------------------------------------
# Goal

Goal is to build an NLP model that can detect tweets about disasters by performing two
tasks that will be combined in a multi-task model.
Given the text of a tweet, we will build NLP models to perform:
1. T1: Disaster detection: classify the tweet into one of two categories: “disaster” or “no
disaster”
2. T2: Sentiment classification: classify the sentiment of the tweet (next slide) to gauge the
severity of the tweet.
We will explore ways to use “signals” from the auxiliary task (sentiment classification) using multitask learning (MTL). MTL is helpful in many occasions — when there are insufficient labelled
samples for the main task, or to improve model performance using auxiliary data in general (even
when there are sufficient labelled samples for the main task). 

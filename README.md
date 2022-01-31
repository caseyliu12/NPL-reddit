# Project 3: Web APIs & NLP

## Problem Statement

In this project, I collect posts from two subreddits (r/boston and r/seattle) using Pushshift's API. The goal of this project is to classify posts from two different subreddits. I will create and compare two models: logistic regression model and random forest model.

Our results may be useful for any reddit individual or business users to see what keywords/contents people are interested most from two cities. We also use sentiment analysis to check if people have postive or negative comments on Boston and Seattle.


## Data Dictionary

The following links are the source of the data used to classify the subreddits.
r/boston: https://www.reddit.com/r/boston
r/seattle: https://www.reddit.com/r/Seattle

|Feature|Type|Description|
|---|---|---|
|**subreddit**|*object*|Which subreddit the post came from.| 
|**selftext**|*object*|Body text of a post.|
|**title**|*object*|Title of a post.| 


## Processing Summary

- Data Collection: Reddit and pushshift.io APIs.
- Data Cleaning & EDA: Clean the data and check the top words from two subreddits.
- Preprocessing & Modeling: Use CountVecorizer with logistical regression model and random forest model while make sentiment analysis.
- Evaluation and Conceptual Understanding: Create confusion matrix and examine classification metrics.


## Conclusion and Recommendations

Our logistic regression model performed well with an accuracy score of 83.39%. The random forest model works equally with score of 82.77%.

Sentiment analysis shows that the comments in r/seattle are slightly positive overall than r/boston. However, we can't conclude which city is better before doing further research.

Future improvements:
 - Choose significantly different subreddits may improve the model.
 - Collect more data sample. Split data in an appropriate way.
 - Include lemmatization, stemming and spell checks to have cleaned post texts.

# Can You Tell Someone’s Gender Based on Tweets?

Predicting someone’s demographic attributes based on limited amount of information available is always a hot topic. It is common to use people’s name, ethnicity, location, and pictures for training models that can tell gender. Can you actually guess someone’s gender only based on what they share on Twitter? We will explore this using NLP techniques in this article.

At the end we conclude that it is quite a challenge to predict someone’s gender only using a single tweet. However, by combining prediction results from many tweets of the same person (similar to ensemble techniques like bagging), we may reach much better performance.

In this study, we applied some NLP techniques (i.e. text pre-processing and TF-IDF features) and built a predictive model that can tell someone’s gender only based on their tweets. Prediction accuracy on a single tweet is 0.59, slightly better than a 50–50 random guess. By combining more tweets from the same person and leveraging majority vote, we were able to achieve much better result.

In the future works, we can try the following to improve prediction accuracy:
* Introduce more tweets for training
* Instead of basic Logistic Regression, try other models such as XGBoost
* Add other features to the data set such as user name, profile bio, etc
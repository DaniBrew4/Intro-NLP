# Intro-NLP
### Introduction to NLP
The “ratings.tsv” dataset is a subset of 8000 movie reviews from a larger dataset of 25,000 movie reviews
(http://ai.stanford.edu/ amaas/data/sentiment/).
The goal is to build a classification model that predicts whether or not the review is positive or negative
based on the words in the review.

1. Import the data. Note that the dataset is tab delimited.
2. Check for and remove missing values and blank strings
3. Split the data into a training set and a test set. Use test size=0.33, stratify=y, and random state=801
(where y is the label positive or negative)
4. Vectorize the data using TD-IDF. Be sure that all model development is with the training data (fit
the TD-IDF transformer on the training data, then transform to both training and test data).
5. Build a machine learning classifier. Try out various models including:
• Support Vector Classifier
• Multilayer Perceptron
• Multinomial Naive Bayes
• (You are welcome to try other models if you want)
6. What model performs the best? Experiment with changing the hyper-parameters, changing the vectorizer, adding bi-grams and/or using a voting classifier to increase model accuracy.
7. If possible, report what words are most important for distinguishing between positive and negative
reviews?
8. Using Vader sentiment analysis, predict whether or not the movie review is positive or negative. (Use
a positive compound score for “positive” and a negative compound score for “negative”).
9. How does the accuracy of the sentiment analysis compare with that of the predictive model?
10. Try doing sentiment analysis with the TextBlob library. How does the accuracy of TextBlob sentiments
compare with Vader and the predictive model?
11. Run LDA topic modeling using gensim on the movie reviews. How many topics are there? What are
the most common words in each topic?

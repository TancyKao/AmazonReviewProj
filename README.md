## How helpful is my review? Predicting review usefulness using machine learning
## Problem
Over the past 10 years, global retail e-commerce has been experiencing an explosive growth. In the world of online market place where touching, smelling or otherwise experiencing products is not feasible, customers heavily rely on other reviewers to make up their minds for a buying decision. However, provided the large volume of reviews, it is important for a website to identify useful, relevant and reliable reviews to help customers save time and make a better choice. Also, useful reviews can help business to increase sales, and improve the product by understanding customers' needs and pain-points.
## Goal
The goal of this project is to mine nine million book reviews from Amazon.com to understand what makes a review helpful to the customer. To this end, a number of models are recruited to test their predictive powers for helpfulness classification of features using the bag of words approach to constructing model features. While our model is built to work with any kind of product, the review dataset provided by Amazon only includes book reviews.
## Data source
http://jmcauley.ucsd.edu/data/amazon/
## Method
We considered review’s star rating, number of words in each review, and useful phrases in the review text to assess their helpfulness. For the useful information of a review, we considered 1,2 and 3 grams as phrases in a text. We used not only “bag of words” to remove non-letters and stop words but also tf-idf (term frequency, inverse document frequency) to get the weighting factors of each phrase. 
## Results
By testing four classifiers, Logistic Regression, Linear Discriminant Analysis, LinearSVC, and Random Forest Classifier, we found that after adjusting the parameters in LR, SVC and RFC algorithms, all models showed better accuracy in predicting helpfulness of a review (64%) compared to shuffled data (51%). We found that the sentiments, such as boring, bad, waste, like and interesting, are good predictors to identify the helpfulness of a review.

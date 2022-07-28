# Movie_reviews_classification_with_BERT
The Film Junky Union, a new edgy community for classic movie enthusiasts, is developing a system for filtering and categorizing movie reviews. The goal is to train a model to automatically detect negative reviews. You'll be using a dataset of IMBD movie reviews with polarity labelling to build a model for classifying positive and negative reviews. It will need to have an F1 score of at least 0.85.

We have completed the following steps in this project:

1.Descriptive statistics

2.Data preprocessing

We removed a few missing values and checked the data for duplicates. We have also normalized the reviews by removing any digits, punctuations marks etc. and converting them to lower case letters.

3.EDA

We analyzed both features and targets. We noticed an overall tendency of the growth of movie reviews over the years, with the peak being in 2006. We found that most often there is just one or a few reviews per movie, although more than 400 movies (probably the most popular ones) have 30 reviews. The overall distributions of ratings among the train and test sets are quite similar, we could probably use this feature in our model.

The distributions of the 2 classes of the train and test sets are very similar - it's a good sign, it means that a model trained on the train set should be predicting correctly on the test set as well. We see that the classes are balanced - there is almost the same amount of positive as well as negative reviews.

4.Splitting the data

Data was split into train and test sets almost equally, according to the preexisting split.

5.Model selection

We have experimented with the 2 types of word embeddings - TF-IDF and BERT. Besides, we tried 2 libraries for text preprocessing - nltk and spaCy. Both Linear Regression and LightGBM models were used.

Model 3 - spaCy, TF-IDF and LR showed the best results with the F1 score being 0.88

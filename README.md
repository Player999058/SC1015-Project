# Movie Genre Predictor

## About this repository
This is a mini project which is an assignment for SC1015 (Introduction to Data Science and Aritificial Intelligence) in NTU. Below are the files that you can found in this repository:

  1. Dataset: [tmdb_5000_movies](https://github.com/Player999058/SC1015-Project/blob/main/tmdb_5000_movies.csv) obtained from Kaggle
  2. Jupyter Notebook: [Movie Genre Predictor.ipynb](https://github.com/Player999058/SC1015-Project/blob/main/Movie%20Genre%20Predictor.ipynb)
  3. Presentation Slides: [Presentation Slides] (https://github.com/Player999058/SC1015-Project/blob/f752d30613c9fcb690559aa7e219b37762d96bfe/PresentationSlides.pdf)

## Problem Definition
To predict the movie genre from the movie overview/plot.

## What's inside our Jupyter notebook?
The Jupyter notebook contains all the code from Introduction to Conclusion. Here is the order in the Jupyter Notebook:

  - Introduction
  - Preliminary Data Cleaning 
  - Exploratory Data Analysis (EDA)
  - Preparation for Machine Learning
  - Machine Learning
  - Insight and Conclusion

## Model Used
1. Dummy Classifier
2. Gaussian Naive Bayes Model
3. Logistic Regression

## Conclusion
* The accuracy of the three models are around 30%, with the highest at 33.04%.
* The problem of having low accuracy is because the dataset is small and the data is quite unbalanced.
* Dummy Classifier actually performed the best compared to other two machine learning technique due to the unbalanced data. Since Dummy Classifier uses the strategy of the most frequency genre, it has a higher percentage of getting the top 2 genres hence the highest accuracy.
* Logistic Regression model performs better than the Gaussian Naive Bayes model with the accuracy almost identical to the accuracy of the Dummy Classifier.
* The confusion matrix plotted confirms the problem where there are many common words among the genres.
* Due to the fact that some of the genres had words in common, false classifications occur most on the genres which have more common words among them.
* Although the accuracy is low, which is at 33.04%, it is still higher than the probability of randomly classifying a movie into one of the genre which is 20%.
* NLTK library is a very powerful library that allows us to analyse words which is considered as unclassified data.
* Natural language processing (NLP) is a very interesting technique to learn and it may be possible to have a higher accuracy to predict the genres if the dataset is large enough or much larger.

## What have we learnt from this project?
* Data cleaning using the method of split by delimiters
* Transforming unstructured data (natural language) into structured data using CountVectorizer
* Using NLTK library methods such as Stopwords
* Generating WordClouds
* Dummy Classifier, Gaussian Naive Bayes Model and Logistic Regression Model from Sklearn
* Exploratory Data Analysis on Categorical Data
* Collaboration using GitHub

## Contributions by Team Members
- Chew You Chun -> Data Cleaning, EDA, Preparation for Machine Learning, Dummy Classifier
- Anson Ang -> EDA, Gaussian Naive Bayes, Logistic Regression

## References
- https://datascienceparichay.com/article/pandas-split-column-by-delimiter/
- https://pythonprogramming.net/tokenizing-words-sentences-nltk-tutorial/
- https://pythonprogramming.net/stop-words-nltk-tutorial/
- https://numpy.org/doc/stable/reference/generated/numpy.select.html
- https://www.sussex.ac.uk/informatics/punctuation/apostrophe/contractions#:~:text=The%20apostrophe%20is%20used%20in,conventional%20items%2C%20mostly%20involving%20verbs.
- https://towardsdatascience.com/why-using-a-dummy-classifier-is-a-smart-move-4a55080e3549
- https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.CountVectorizer.html
- https://www.statology.org/seaborn-barplot-show-values/

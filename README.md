# Intelligenza-Artificiale
Mirko Del Moro - 6368874

We use the Naive Bayes implementations for the problem of sentiment analysis with drug reviews.

# Requirements
- scikit-learn
- pandas
- numpy
- string
- re

# Preprocessing
- remove punctuation, numbers and special characters
- all alfabetic characters convert to lowercase

# Vectorization
We use CountVectorizer() function to transform the extracted text in a sparse matrix of features
- ngram-range(): min and max number of word considered to represent the text
- max_df(): terms with a document frequency higher than a given threshold are discarted

# Naive Bayes
We initialize and fit MultinomialNB and BernoulliNB and use them to predict the test.

# Results
Print the accuracy, the cohen's Kappa and the confusion matrix for both models.


For reproduce the results in sentiment_analysis.ipynb you need to load the dataset from http://archive.ics.uci.edu/ml/datasets/Drug+Review+Dataset+%28Drugs.com%29 and modify the path in pandas.read_table() function.

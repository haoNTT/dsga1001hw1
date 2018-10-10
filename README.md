# dsga1001hw1

This is the first homework assignment of DS-GA 1011 Natural Language Processing. 

A program is established to perform sentimental analysis to movie reviews from IMDB dataset. The dataset is available at: http://ai.stanford.edu/~amaas/data/sentiment/ 

The movie reviews applied in this program are all from IMDB dataset which consisting 50000 movies.
Half of these movies are used as testing set and the other half of the movies are split into a training set
with 20000 movies and a validation set with 5000 movies.

The program has two versions. The basic version established a binary classifier to classify the sentiment
scores into positive or negative. The advanced version established a model which tries to classify movie
reviews according to their labeled sentimental scores from 0 to 10.

For both versions, standard data preprocessing techniques are applied to clean the input data. All
input movie reviews are tokenized with punctuations removed. A vocabulary is established which contains
specified number of most frequent tokens. Then two lookup tables are set up so that the tokenized datasets
can be converted into datasets represented in indices which are ready to serve as input to machine learning
models. Finally, a bag-of-words model is set up to convert input tokens by the embedding layers and then
the results are fed into a logistic regression model to perform classification.
The advanced version of this program is designed to predict the rating of movie reviews with scores
range from 0 to 10. The files are loaded according to their scores and the label sets are established
correspondingly. The model used to perform the prediction is a two-layer neural network which applies
Relu and Softmax activation functions.
In order to detect the influence of different choices of hyper-parameters to the general accuracy of the
model, different tokenization schemes are applied. In this program, there are two versions of tokenization
which are named as basic tokenization and advanced tokenization. The basic tokenization applies SpaCy
package to tokenize the movie reviews with only punctuations removed while the advanced tokenization
applies NLTK to have punctuations and stop words removed from tokens. The advanced tokenization also
applied word stemming to unify the format of words.

Please check the code to look for anything in details 

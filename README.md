# Find Movie Similarity from Plot Summaries

this is a datacamp project with the goal of finding similarities between movies
based on their plot summary which we can found on imdb and wikipedia combined to 
increase accuracy and provide more details

we start by the basic NLP process: 
1- Tokenizing sentences and then words and getting rid off punctuation and numeric values
2- Stemming these words to get the root of each because that's what matters most

and then we create the TF-IDF vectorizer which will both determine the most important 
words for each movie and ommit the words that are present in all of the plots such as the frequent words

after fitting and transforming our texts into vectorizers, we've got our TF-IDF matrix
that we'll group its data to clusters using the KMeans algorithm

then, for visualising purposes, we've got to calculate the similarity distance between all the movies
according to the values present in the tf-idf matrix

which will help us afterwards show our dendrogram

# # Frameworks Used

numpy, pandas, nltk, sklearn, matplotlib

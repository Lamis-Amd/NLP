## Document representation
### How to represent a document?
Make it computable
### How to infer the relationship among documents or identify the
structure within a document?
Representation is the first, probably the most important and
most complex problem in almost all Natural Language
Processing (NLP) tasks.
Representation aims to numerically represent unstructured text
documents as word vectors to make them mathematically
computable.
### Pre-processing
In any machine learning task, preprocessing or cleaning the
data is as important as model building .
Some of the common text preprocessing / cleaning steps are:
Lower casing
Removal of Punctuations
Removal of Stopwords
Stemming, Lemmatization
#### Spelling correction: which this repository focuses on:
We define a function correct_spelling that takes an input word and a list of words as arguments.
The function calculates the Levenshtein distance (a measure of the difference between two strings) between the input word and each word in the list using the levenshtein.normalized_distance() function from the textdistance library.
The list of distances is then sorted in ascending order.
The word with the lowest Levenshtein distance (i.e., the word that is most similar to the input word) is returned as the corrected spelling.
We provide an example usage where we specify a list of words for testing and an input word with a misspelling. The code then corrects the spelling of the input word and outputs the corrected word.

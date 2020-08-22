
Completition
https://www.kaggle.com/c/nlp-getting-started/overview

Problem: 
Given: a text of a tweet and some metadata (Location and Keyword)
Find: if the tweet talks about real disaster


Motivations:
Monitor the situation in a real time
- Quick
- Inexpensive
- Safe
Predict a follow-up process
Real situation from contradicting tweets
Categorization of situational and conversational data is important



Pre-Processing Data:
- Convert text to lowercase
- Remove stopwords
- Remove punctuation
- Remove digits
- Text vectorization (TF-IDF transformation)


Vocabulary Embedding Coverage:
- GloVe (300d)
- Google Negative(300d)
Some of the words not included in the embedding dictionary.


Baseline Model:
- Vectorize the Text and Calculate the Frequency of each word 
from sklearn.feature_extraction.text import TfidfVectorizer
- Collect Features from TfidfVectorizer (without semantics)
(Term Frequency–Inverse Document Frequency)
tfidf(t,d,D) = tf(t,d) * idf(t, D)
-Model : Logistic Regression and Support Vector Machine 

Results: Kaggle Leaderboard:
No. 330 at 0.84 error.

Kaggle submittion:
https://www.kaggle.com/kirilkuzmin/svm-with-words2vectors-mapping
https://www.kaggle.com/henryascend/shiba-innu-of-bert-henry
https://www.kaggle.com/martofthenorth/glove-twitter-with-lstm-mart

MODELS:
Long Short term Memory -  LSTM 
Bidirectional Encoder Representations from Transformers - BERT 
WORD2VEC


Conclusion:

1. Some tweets have contradictory labels
2.BERT showed the best results: 
- public score: 0.8425
- accuracy = 0.8774  f1 = 0.8474 precision = 0.8759 recall = 0.8276
3. Word2Vec is next:
- public score: 0.8108
- accuracy = 0.8244 f1 = 0.8219 precision = 0.8270 recall = 0.8244
4. Tomáš Mikolov is smart
5. Sometimes it can go off…
6. We have learnt:
- how to use Kaggle platform
- way to clean text data
- NLP
- shallow vs deep models for NLP
- how to work in a team



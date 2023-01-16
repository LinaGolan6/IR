# IR

This code performs text retrieval using the TF-IDF algorithm. 

The storage library is from Google Cloud to access data stored in a Google Cloud Storage bucket. 
NLTK library used to perform tokenization and stopword removal.

The code first defines a function that use the storage library to create access a bucket on Google Cloud Storage. 

It also use NLTK's list of stopwords, which are used in the tokenize function to remove common words from the text that don't have much meaning.

The code then defines several functions to perform text retrieval: 
The tokenize function tokenizes a given text and removes stopwords, get_candidate_documents_and_scores retrieves candidate documents and their scores, 

binary_search function is used to find the similarity between the query and the documents.

tfidf_candidates and tfidf_query function is used to calculate the tf-idf score of candidate documents and query to rank them.

Finally, binary_search function is used to find the similarity between the query and the documents.

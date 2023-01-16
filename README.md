# IR

This code performs text retrieval using the TF-IDF algorithm. It uses the hashlib and pickle libraries to process data, the storage library from Google Cloud to access data stored in a Google Cloud Storage bucket, and NLTK library to perform tokenization and stopword removal.

The code first defines a function _hash that creates a hash of a given string using the blake2b algorithm. Then, it uses the storage library to create a client and access a specific bucket on Google Cloud Storage. It then retrieves two files from the bucket, 'Body_index.pkl' and 'body_idf.pkl' and loads them into memory using the pickle library.

It also uses nltk.download('stopwords') to download NLTK's list of stopwords, which are used in the tokenize function to remove common words from the text that don't have much meaning.

The code then defines several functions to perform text retrieval. The tokenize function tokenizes a given text and removes stopwords, get_candidate_documents_and_scores retrieves candidate documents and their scores, get_candidate_documents_and_scores_search retrieves candidate documents, tfidf_candidates calculates the TF-IDF scores for the candidates, and tfidf_query calculates the TF-IDF scores for the search query.

binary_search function is used to find the similarity between the query and the documents.

get_candidate_documents_and_scores and get_candidate_documents_and_scores_search function is used to get the candidate documents based on the query and index.

tfidf_candidates and tfidf_query function is used to calculate the tf-idf score of candidate documents and query to rank them.

Finally, binary_search function is used to find the similarity between the query and the documents.

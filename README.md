# Latent-Dirichlet-Allocation

In machine learning and natural language processing, a topic model is a type of statistical model for discovering the abstract "topics" that occur in a collection of documents. Topic modeling is a frequently used text-mining tool for discovery of hidden semantic structures in a text body. Intuitively, given that a document is about a particular topic, one would expect particular words to appear in the document more or less frequently: "dog" and "bone" will appear more often in documents about dogs, "cat" and "meow" will appear in documents about cats, and "the" and "is" will appear approximately equally in both. A document typically concerns multiple topics in different proportions; thus, in a document that is 10% about cats and 90% about dogs, there would probably be about 9 times more dog words than cat words. The "topics" produced by topic modeling techniques are clusters of similar words. A topic model captures this intuition in a mathematical framework, which allows examining a set of documents and discovering, based on the statistics of the words in each, what the topics might be and what each document's balance of topics is.




About LDA



LDA is used to classify text in a document to a particular topic. 


It builds a topic per document model and words per topic model, modeled as Dirichlet distributions.


Each document is modeled as a multinomial distribution of topics and each topic is modeled as a multinomial distribution of words.



LDA assumes that the every chunk of text we feed into it will contain words that are somehow related. Therefore choosing the right corpus of data is crucial.



It also assumes documents are produced from a mixture of topics. Those topics then generate words based on their probability distribution.


To learn more about LDA please check out this link.



Extracting Topics using LDA in Python



Preprocessing the raw text


This involves the following:


Tokenization: Split the text into sentences and the sentences into words. Lowercase the words and remove punctuation.


Words that have fewer than 3 characters are removed.


All stopwords are removed.


Words are lemmatized — words in third person are changed to first person and verbs in past and future tenses are changed into present.


Words are stemmed — words are reduced to their root form.



We use the NLTK and gensim libraries to perform the preprocessing

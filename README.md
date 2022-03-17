The goalis enabling computers to interpret, analyze, and approximate the generation of human languages.

NLP got its start around 1950 with Alan Turing’s test for artificial intelligence evaluating whether a computer can use language to fool humans into believing it’s human.

Python has some of the most extensive open-source NLP libraries, including the Natural Language Toolkit or NLTK.
1. Text preprocessing
    - Noise removal — stripping text of formatting (e.g., HTML tags).

    - Tokenization — breaking text into individual words.

    - Normalization — cleaning text data in any other way:

                Stemming is a blunt axe to chop off word prefixes and suffixes. “booing” and “booed” become “boo”, but “computer” may become “comput” and “are” would remain “are.”
                Lemmatization is a scalpel to bring words down to their root forms. For example, NLTK’s savvy lemmatizer knows “am” and “are” are related to “be.”
                Other common tasks include lowercasing, stopwords removal, spelling correction, etc.

2. Language Models:We can help computers make predictions about language by training a language model on a corpus (a bunch of example text).
    a. Bag-of-Words (unigram model), tally count of each instance for each word.
    Bag-of-words can be an excellent way of looking at language when you want to make predictions concerning topic or sentiment of a text. When grammar and word order are irrelevant, this is probably a good model to use.

    b. N-Gram : he n-gram model considers a sequence of some number (n) units and calculates the probability of each unit in a body of language given the preceding sequence of length n. Because of this, n-gram probabilities with larger n values can be impressive at language prediction.
    For a model that more accurately predicts human language patterns, you want n (your sequence length) to be as large as possible. That way, you will have more natural sounding language. Well, as the sequence length grows, the number of examples of each sequence within your training corpus shrinks. With too few examples, you won’t have enough data to make many predictions.

    c.Topic Models
    Topic modeling is an area of NLP dedicated to uncovering latent, or hidden, topics within a body of language. latent Dirichlet allocation (LDA). LDA is a statistical model that takes your documents and determines which words keep popping up together in the same contexts (i.e., documents). We’ll use sklearn to tackle this for us.word2vec can map out your topic model results spatially as vectors so that similarly used words are closer together.

Text similarity
    Levenshtein distance = minimal edit distance between two words (turning “bees” into “beans” would require one substitution (“a” for “e”) and one insertion (“n”), so the Levenshtein distance would be two.)
Phonetic similarity
Lexical similarity
Semantic similarity

Language prediction
   Pick a model
     bag of words (not enugh)
     Markov chains (n-gram)Markov chains are memory-less and make statistical predictions based entirely on the current n-gram on hand.
     Long Short Term Memory (LSTM) - neural l.model. LSTM uses deep learning with a network of artificial “cells” that manage memory, making them better suited for text prediction than traditional neural networks.

 Naive Bayes classifiers are supervised machine learning algorithms that leverage a probabilistic theorem to make predictions and classifications. They are widely used for sentiment analysis (determining whether a given block of language expresses negative or positive feelings) and spam filtering.    
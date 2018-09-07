# Topic_modelling
Topic Modelling Using Scikit, for IMDB movie rating


Topic modelling can be described as a method for finding a group of words (i.e topic) from a collection of documents that best represents the information in the collection. It can also be thought of as a form of text mining – a way to obtain recurring patterns of words in textual material

Latent Dirichlet Allocation (LDA)
In the LDA model, each document is viewed as a mixture of topics that are present in the corpus. The model proposes that each word in the document is attributable to one of the document’s topics.


Process Explained:

Go through each document and randomly assign each word in the document to one of K topics (K is chosen beforehand)
This random assignment gives topic representations of all documents and word distributions of all the topics, albeit not very good  ones

So, to improve upon them:
         For each document d, go through each word w and compute:
         p(topic t | document d): proportion of words in document d that are assigned to topic t
         p(word w| topic t): proportion of assignments to topic t, over all documents d, that come from word w

Reassign word w a new topic t’, where we choose topic t’ with probability
    p(topic t’ | document d) * p(word w | topic t’)
    This generative model predicts the probability that topic t’ generated word w





Data Used

link - http://ai.stanford.edu/~amaas/data/sentiment/
ACL paper - 2011, 
Author = = {Maas, Andrew L.  and  Daly, Raymond E.  and  Pham, Peter T.  and  Huang, Dan  and  Ng, Andrew Y.  and    
            Potts, Christopher},
title     = {Learning Word Vectors for Sentiment Analysis}

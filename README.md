Word Embedding + Question Answering Tranformer

In this project, I have used word embeddings to retrieve the most relevant documents from the nlp-pipeline processed dataset. The dataset I have selection are the HTML
pages from People Law Library (https://www.peoples-law.org/). Through initial testing, the embeddings perform better than Solr and Elastic Search. 

After retrieving these documents with the "relevancy" scores, I have used the document content and passed it to the model "deepset/roberta-base-squad2" to recieve the 
generalized answer of the question. The answer is evaluated on the score which is used as confidence, to either provide a answer to the question or pass it to 
another transformer which will summarize the page content. 

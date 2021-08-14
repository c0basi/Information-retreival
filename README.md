# Information-retreival

Simple implementation of an Information Retrieval (IR) system based for a collection of documents (Twitter messages),

The system make use of the BERT and Glove model to rank results 

#1 In this step, we have used the Bert model for the representation of documents. It has been provided by the Python’s library of sent2vec. Bert is a deep learning based model which can be used as word embedding. It has encoder–decoder based architecture with 12 layers in the encoder and 12 layers in the decoder. Because of being so deep, it usually take a large time for training. 


#2 In the second experiment we have used Glove for the word representation unlike a Bert which is a model for sentence representation. Glove which stands for Global Vectors represent words using word-context co-occurrence matrices. In the code we have use the pre-trained glove word embedding, provided by the gensim library, which is present under the name ‘glove-twitter-200’. As the name suggests, this pre-trained embedding represent the words by a 200 dimensional vector and was trained on a twitter data. The main idea here is that the similar words will lie close to each other in this dimensional space. This expects the documents in the form of tokens separated by comma. 


###
# Instructions on How to Run the Program
The program can be run in Jupyter Notebook or in the Google Colab Environment. It has been required to upload three files before running the program. First is to Trec_microblog11.txt which will contains the documents or in the other words it will contain the training data. Second file, topics_MB1-49.txt, will contain the testing queries for which we want to select the mot similar documents. Third file will be assign1_Results.txt, it will contain the results from assignment 1 as we want to re-rank these documents for experiment 1 which was of a Bert model.  

# Results File
In this step, we had to run the set of 49 Twitter message test queries on our system. However, we needed to return the results in TREC format and then store them into a .txt file called Results. Moreover, only the top 1000 results for each query would be stored with the queries ordered in ascending order. This was done for both experiments, but the one with best results was chosen to submit.


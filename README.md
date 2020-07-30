# US-Election 2020 Result Prediction : Project Overview
* Created a tool that predicts the result of US-Election 2020 .
* Scraped over 50 thousand tweets using twitter streaming API.
* Engineered features from the json data by extracting important features into CSV file.
* Preprocessed the tweets using NLP to overcome noise from the dataset.
* Labeled the Tweets according to the polarity of the tweet using Lexicon based algorithm.
* Generated word embeddings using Word2Vec algorithm with CBOW architechure and trained 300 dimensional embeddings.
* Performed unsupervised machine learning, k means clusterning to cluster the embedding according to their polarity.
* Calculated the final Result based on the analysis of the tweets.


## Motivation
The prolifertion of social media on recent past has provided end users a powerfull platform  like facebook twitter and Instagram.
These platform are actively being used to share ratings reviews and recommendations.These platmorm also allows users to express there 
political opinions.In this project we have used sentiment analysis to analysize 50k tweets to predict USElection result 2020. 
The sentiment analysis of text combines natural language processing and machine learning techniques to assign weighted sentiment scores to entities 
topics and themes in the sentence.
  
## Code and Resources Used
**Python Version:** 3.7
**Packages:** pandas numpy sklearn json csv word2vec tweepy sklearn gensim nltk

## Data Collection
   The data for this project is collected for two candidates namely Donald trump and Joe Biden using twitter streaming data.
   
   
### Data Preprocessing
 * In this stage, The tweets were stripped off special characters, URL's, usermentions and punctuations to overcome noise.
   secondly the stopwords were removed from the dataset and the words were lemmatized into their root words.
 * Since the negative and positive words are surrounded by similar words, word2vec algorithm with CBOW architechure and trained 300 dimensional embeddings to find relation
   b/w words and created w2v model.
      
   word2vec takes a large corpus of text as input and produces a vector space of several hundred dimensions with each unique word in corpus being assigned
   a corresponding vetor in space. Word vectors that share common context in the corpous are located close to each other in space.
   
      
## Model Building
   * This project presents two algorithms to analyse Twitter data for prediction:
     **1. Lexicon based algorithm:** Use of VADER lexicon to find the polarity of the sentence.
     **2. Unsupervised Machine Learning:** Implemented Machine learning on the Word2vec model using the K-Means Clustering algorithm.
          Here 2 centriods are assigned for positive  and negitive opinions and k means algorithm allocates every data point to the nearest cluster. Then words are assigned a
          sentiment score based on the cluster they belong or how close they are to that cluster.
          
          
 ## What I learned
   Cleaning and Preprocessing the raw data is a challange in itself and the most important part of any Machine learning process. 
   Because only if the data is free from any noiseand is properly preprocessed, we can achieve the desired result.
   Through this project I Learnt concepts of Natural Language Processing and unsupervised Machine learning.I got hand-on experience on working with raw data,
   preprocessing data and removing noise from data and then predicting the outcome.
    
    
 
    
    
    


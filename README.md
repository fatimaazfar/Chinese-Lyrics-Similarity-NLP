# Chinese Language Similarity - NLP

Welcome to the Chinese Language Similarity project! This project focuses on finding similarities between Chinese language sentences and lyrics using Natural Language Processing (NLP) techniques. The code explores various methods, including TF-IDF, BERT embeddings, and a Bidirectional Temporal Siamese Network.

## Table of Contents
- [Introduction](#introduction)
- [Environment Setup](#environment-setup)
- [Exploratory Data Analysis (EDA)](#eda)
- [Preprocessing](#preprocessing)
- [TF-IDF and Cosine Similarity](#tf-idf-and-cosine-similarity)
- [BERT Embeddings](#bert-embeddings)
- [Bidirectional Temporal Siamese Network](#bidirectional-temporal-siamese-network)
- [Data Cleaning](#data-cleaning)
- [Cleaned Data - Siamese Network](#cleaned-data-siamese-network)
- [Data Availability](#data-availability)

## Introduction
This project aims to compare the similarity between Chinese language sentences or lyrics. It employs various NLP techniques to process and analyze the data, providing insights into the semantic similarity between different pieces of text.

## Environment Setup
Make sure you have the required libraries installed. You can install them using the following commands:

```bash
pip install pandas nltk beautifulsoup4 scikit-learn jieba
pip install bert-serving-server bert-serving-client
pip install keras tensorflow
```

## Exploratory Data Analysis (EDA)
The initial phase involves exploring the dataset using pandas and performing basic EDA to understand its structure. The dataset is loaded from an Excel file named "Lyrics Test.xlsx," and specific operations are performed on the data related to a song with the ID 1835514122.

## Preprocessing
Text data preprocessing is a crucial step to enhance the quality of analysis. The code includes functions to clean English and Chinese lyrics by removing unnecessary elements such as punctuation, stopwords, and numbers. It utilizes libraries like NLTK, Jieba, and regular expressions for efficient text processing.

## TF-IDF and Cosine Similarity
The TF-IDF vectorization technique is employed to convert the lyrics into numerical vectors. Cosine similarity is then used to measure the similarity between different songs based on their TF-IDF representations.

## BERT Embeddings
The code demonstrates the use of BERT embeddings to represent the semantic meaning of Chinese lyrics. It utilizes the BERT serving server and client for efficient processing.

## Bidirectional Temporal Siamese Network
A Siamese Network is implemented using Keras to learn the similarity between pairs of song lyrics. This neural network architecture utilizes bidirectional LSTM layers and an attention mechanism to capture temporal dependencies in the lyrics.

## Data Cleaning
A cleaned version of the dataset is created by removing noise, such as pure instrumental tracks and 'N/A' values in Chinese lyrics.

## Cleaned Data - Siamese Network
The cleaned dataset is then used to train the Bidirectional Temporal Siamese Network, providing improved similarity results without non-Chinese lyrics noise.

## Data Availability
The data is not publicly available for now.

Feel free to explore the code and adapt it to your specific use case. If you have any questions or suggestions, please don't hesitate to reach out.

Happy coding! 🚀

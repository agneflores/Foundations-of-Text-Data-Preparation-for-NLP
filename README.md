# Foundations of Text Data Preparation for NLP
The project notebook can be found 

### Project Overview
This project delves into the fundamental aspects of preparing text data for natural language processing (NLP) models. It encompasses various techniques including word and sentence tokenization, lexical diversity, and text manipulation within DataFrames. The notebook provides a comprehensive guide on opening and processing .txt files, handling parts of speech, named entity recognition, and text preprocessing techniques such as stemming and lemmatizing. By exploring these foundational methods, the project equips users with essential skills for effectively managing and analyzing text data in NLP applications.

______________________________________________________________________________________________________________________________________________________________________________________________________________________________

### Data
The notebook will use both a single piece of text in the form of a lead paragraph from Isaac Newton's *Principia* and a dataset including text data from [kaggle](https://www.kaggle.com/datasets/sankha1998/emotion?select=Emotion%28sad%29.csv) related to classifying WhatsApp status. 

______________________________________________________________________________________________________________________________________________________________________________________________________________________________

### Part 1: Tokenization

This notebook focuses on tokenizing text.  It will use `nltk` to tokenize words and sentences of a given document.  In general, tokenizing a text refers to the operation of splitting the text apart into chunks.  Here, our chunks can be individual "words" and "sentences".  These are not necessarily meant to refer to proper grammatical structure or meaning, however splitting entities based on white space, periods, or other punctuation.  

#### Outline

- Word Tokenizing a String
- Sentence Tokenization of a string
- Unique Words with 'set'
- Counts of words
- Lexical Diversity
- Text in a DataFrame

______________________________________________________________________________________________________________________________________________________________________________________________________________________________

### Part 2: Named Entities

This part of the notebook focuses on extracting named entities from text.  The named entities will be extracted using the `nltk` library.  It will read in the full text of Newton's *Principia* and identify the entities labeled as places.  

#### Outline

- Opening a `.txt` file
- Tokenizing the text
- Part of Speech Tags 
- Named Entities
- Removing People
- Removing stopwords

______________________________________________________________________________________________________________________________________________________________________________________________________________________________

### Part 3: Stemming and Lemmatization

In this part, notebook will stem and lemmatize a text to normalize a given text. It will use the lemmatizer and stemmer on a basic list and then turn to data in a DataFrame, writing a function to apply the lemmatization and stemming operations to a column of text data.  The data is the WhatsApp status dataset from kaggle, and notebook will focus on the `content` feature.

- Stemming a list of words
- Lemmatizing a list of words
- A function for stemming
- Using the stemmer on a DataFrame

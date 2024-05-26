# Emotions Analysis

## Introduction

Welcome to the "Emotions" dataset – a collection of English Twitter messages meticulously annotated with six fundamental emotions: anger, fear, joy, love, sadness, and surprise. This dataset serves as a valuable resource for understanding and analyzing the diverse spectrum of emotions expressed in short-form text on social media.

## About the Dataset

Each entry in this dataset consists of a text segment representing a Twitter message and a corresponding label indicating the predominant emotion conveyed.
The emotions are classified into six categories:

+ Sadness (0)
+ Joy (1)
+ Love (2)
+ Anger (3)
+ Fear (4)
+ Surprise (5)

Whether you're interested in sentiment analysis, emotion classification, or text mining, this dataset provides a rich foundation for exploring the nuanced emotional landscape within the realm of social media.

# Key Features

+ text: A string feature representing the content of the Twitter message.
+ label: A classification label indicating the primary emotion, with values ranging from 0 to 5.

# Potential Use Cases

+ Sentiment Analysis: Uncover the prevailing sentiments in English Twitter messages across various emotions.
+ Emotion Classification: Develop models to accurately classify tweets into the six specified emotion categories.
+ Textual Analysis: Explore linguistic patterns and expressions associated with different emotional states.

# Data Preprocessing

+ Imported necessary libraries including pandas, numpy, matplotlib, BeautifulSoup, regex, string, TextBlob, nltk, and emoji.
+ Preprocessed text data by:
  * Converting to lowercase
  * Removing HTML tags, URLs, punctuation, and chat words
  * Applying lemmatization
  * Removing stopwords and emojis

# Tokenization and Padding

+ Tokenized text data and performed padding to ensure uniform length for input sequences.

# Model Architecture
Utilized a deep learning architecture comprising:

+ Embedding layer with bidirectional LSTM (Long Short-Term Memory)
+ Batch normalization and dropout layers for regularization
+ Dense layers with ReLU activation
+ Output layer with softmax activation
Compiled the model using the Adam optimizer and sparse categorical crossentropy loss.

# Model Training

+ Trained the model on the preprocessed and tokenized text data for 5 epochs with a batch size of 128.
+ Evaluated model performance using validation data.




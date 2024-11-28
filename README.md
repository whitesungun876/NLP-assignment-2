# NLP Assignment: Morphology, Language Models, Edit Distance, and Sentiment Analysis

This repository contains solutions for a series of Natural Language Processing (NLP) exercises. The exercises cover multiple topics, including morphology, language models, minimum edit distance, and sentiment analysis using Naive Bayes. Below is a summary of the tasks completed in this assignment.

## Part 1: Morphology

### Exercise 1.1: Part-of-Speech Tagging for English
- Used `nltk.pos_tag` to Part-of-Speech tag English texts.
- Extracted words in present tense and past tense.

### Exercise 1.2: POS Tagging for Spanish (Extra)
- Trained a POS tagger for Spanish and extracted words in present tense and past tense.

## Part 2: Language Models

### Exercise 2.1: Training Language Recognizers using Character Bigrams
- Trained language models for English, Spanish, and an additional language of choice using character bigrams.
- Utilized NLTK’s `ConditionalFreqDist` to create bigram frequency distributions.
- Converted the frequency distributions into conditional probability distributions using Maximum Likelihood Estimation (`MLEProbDist`).

### Exercise 2.2: Sentence Probability Prediction
- Provided 3 example sentences and predicted the probability of each sentence belonging to the trained language models (English, Spanish, and the third language).
- Analyzed the effectiveness of these language models for language recognition, particularly for short texts.

## Part 3: Minimum Edit Distance (MED)

### Exercise 3.1: Extending MED Implementation
- Extended the provided Minimum Edit Distance (MED) implementation to return a single alignment.
- The alignment consists of a sequence of actions such as deletion (d), insertion (i), substitution (s), and no change (-).

### Exercise 3.2: Present vs Past Tense Differences using MED
- Used the MED method to compare verb pairs in present and past tense (e.g., play-played, run-ran, como-comí).
- Analyzed the differences between present and past tense in different languages, including the language of choice (optional).

## Part 4: Sentiment Analysis

### Exercise 4: Implementing Naive Bayes Sentiment Analysis

#### Exercise 4.1: Calculating Prior Probabilities
- Calculated prior probabilities for the positive and negative classes in movie reviews using log probabilities (as discussed in class).

#### Exercise 4.2: Word Count Calculation for Positive and Negative Reviews
- Calculated the word counts for positive and negative reviews separately and stored them in dictionaries.

#### Exercise 4.3: Estimating Word Probabilities
- Estimated the log probability of each word appearing in positive and negative reviews.

#### Exercise 4.4: Handling Out-of-Vocabulary (OOV) Words
- Estimated the log probability for out-of-vocabulary words for both positive and negative reviews.

#### Exercise 4.5: Sentiment Prediction Function
- Implemented a function that predicts whether a review is positive or negative based on the trained Naive Bayes model.

## Files:
- `en.txt` - Raw English text data used for Part 1 and 2.
- `sp.txt` - Raw Spanish text data used for Part 1 and 2.
- `xx.txt` - Raw text data for the third language used in Part 1 and 2.
- `EN_mytok_red.txt` - Tokenized version of the English text (first 2000 tokens).
- `EN_NLTK_tok.txt` - NLTK tokenized version of the English text (first 2000 tokens).
- `EN_preproc.txt` - Pre-processed English text (stopwords removed).
- `sentiment_model.py` - Python script for training and evaluating the Naive Bayes sentiment analysis model.

## Insights:
- The Part-of-Speech tagging and language models offer insights into tense usage in different languages and how well character bigrams can classify short texts by language.
- The Minimum Edit Distance analysis helped identify systematic transformations in verb forms (present vs past tense) across languages.
- Sentiment analysis was successfully implemented using Naive Bayes, with techniques for handling word counts, log probabilities, and out-of-vocabulary words.

## Requirements:
- `nltk`
- `numpy`
- `scikit-learn` (for Naive Bayes)

## Installation:
To install the required dependencies, run:

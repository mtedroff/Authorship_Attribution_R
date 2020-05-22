# Authorship Attribution in R

This study is part of the course SECU0057 Applied Data Science at UCL, and aims to classify the author of a given text accurately. This corpus contains 10 bloggers with 500 data points each, where one data point contains 400-1500 words. Data was collected through web-scraping 10 individual blogs covering topics related to venture capital, technology, and entrepreneurship. In this corpus, several standard stylometric variables were calculated, including word length, vocabulary diversity, word frequency, and n-grams, including bigrams and trigrams. A Naïve Bayes classifier algorithm was trained on the data set together with TF-IDF as a feature selection method. It had an accuarcy of 0.826 on the testing data. It can 82.60% accurately identify authors based on text.

# Background

Authorship attribution refers to identifying an author for a given piece of text. In the past decades, automatic authorship identification has been increasingly popular among researchers in artificial intelligence, computing, linguistics, humanities, security, law, and theology. Authorship classification has been applied in various areas, from online posts to digital forensics and fraud detection and poetry (see, e.g., Chaski, 2005; Iqbal et al., 2008;  Zheng et al., 2006; Ahmed, Mohamed, and Mostafa, 2019).

As of 2020, there are approximately 600 million blogs worldwide. Authorship attribution for online documents differs slightly from traditional work in many ways, as texts are commonly more unstructured and less compliant with grammatical rules, using free-form sentences and a more subjective tone (Mischne, 2007). Blog language is attractive among researchers in the linguistic community as it combines personal views, monologue, dialogue, news, or reporting on current events (Mischne, 2007).

# Method and Process

R Packages used: jsonlite, rvest, stringr, svMisc, readxl, tidyr, quanteda, caret, ggplot2, quanteda_textmodels, tidyverse, pander, e1071

Data Collection:
- Web-scraping of 10 individual blogs

Stylometric Analysis:
- Distribution of no of Sentences, Distribution of number of sentences by Author, Average sentence length, Distribution of Number of Words by Author, Average number of words by author, Word Length by Author, Average Vocabulary Size by Author, Average number of commas, Vocabulary diversity by constructing a document-feature matrix (DFM)  Vocabulary diversity using type token ratio, TTR, Word frequency and most used words,	N-grams analysis (bigrams and trigrams)

Text pre-processing:
- Removal of stopwords & punctuation, tokenization, stemming, TF-IDF

Classification:
- Naïve Bayes classifier algorithm  with TF-IDF


# Future Work

Future work could investigate the robustness of other algorithms for authorship attribution and compare multiple classifiers and feature selection methods, including generative and discriminative models.

The feature and linguistic properties analysis can be expanded. Since the paper studied online blog posts, factors such as number of emojis used, topical diversity, gender of the author, syntactical features including characterized that are capitalized, number of special characters, no upper-case letters and quotation marks, to fully capture the personality and richness of this medium. 


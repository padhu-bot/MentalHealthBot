# MentalHealthBot

## Table of Contents

- [Text Pre-processing](#text-pre-processing)
- [Text Exploration](#text-exploration)
- [Wordcloud](#wordcloud)
- [Labelling](#labelling)
- [Modeling](#modeling)
- [Testing](#testing)

### Text Pre-processing

For text pre-processing, we followed these steps:
- Lowercasing: All text was converted to lowercase for consistency.
- Remove-number: To eliminate numerical digits from the text, I used the isdigit method to remove all numeric characters.
- Removing Punctuations: I removed punctuation marks from the text using a list of common punctuation characters.
- Space removal: I stripped leading and trailing whitespace from the text to ensure uniform formatting.
- Special Characters: Special characters removed using regular expressions.
- Duplicate removal: I removed duplicate words within the text to simplify and clean it further. 
- Stopword Removal: Common English stopwords were removed to reduce noise.
- Lemmatization: We employed NLTK for lemmatization to reduce words to their base form.

### Text Exploration

-Tokenization: 
Tokenization is the process of breaking down text into individual words or tokens. We performed tokenization on the raw text data to prepare it for further analysis.

-Frequency Distribution:
To understand the frequency of words in the text corpus, we used the Frequency Distribution (FreqDist) module from NLTK. FreqDist allows us to count the occurrences of each word in the corpus.

### WordCloud:
To visually represent the most frequently occurring words in our text corpus, we generated a word cloud using a library like WordCloud in Python. The word cloud provides an intuitive snapshot of the most prominent terms.

### Labelling

Label encoding assigns a unique numerical label to each category or answer which is the target value. This numerical representation makes it easier for the chatbot to manage and generate responses, as it can work with numerical values more efficiently than with text.

### Modeling

I am using the basic SVC model with standard param to train the FAQ data.

###  Testing 

I am testing my model with few similar user questions and checking manually if they give relevant answers


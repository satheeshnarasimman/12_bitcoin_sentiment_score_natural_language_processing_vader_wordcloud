# week12_nlp_project
In this project, the latest news articles of Bitcoin and Ethereum are analyzed via Natural Language Processing (NLP) methods such as Sentiment Intensity Analyzer, Tokenization, WordCloud and Named Entity Recognition (NER).

## Libraries/ Technologies used
- os
- numpy
- pandas
- load_dotenv
- newsapi
- nltk
- SentimentIntensityAnalyzer
- matplotlib
- matplotlib.pyplot
- vader_lexicon
- word_tokenize
- sent_tokenize
- stopwords
- WordNetLemmatizer
- from string, punctuation
- re (regular expression)
- Counter
- ngrams
- WordCloud
- spacy
- displacy

## Tools used
- Github
- Gitbash
- Gitlab
- Slack
- Jupyterlab
- NewsAPI

## Data Fetched
- Latest news about Bitcoin and Ethereum from NewsAPI

## High-level summary
### Section 1- Sentiment analysis
- The news about Bitcoin and Ethereum is fetched via NewsAPI.
- Two lists are created to hold the Bitcoin and Ethereum sentiment scores and article text. The respective lists are converted to a Pandas DataFrame.
- The summary statistics of the sentiment scores are calculated.

### Section 2- Tokenization
- A tokenizer master function is defined that removes the stopwords, non- alpha numeric characters, lemmatizes the news text and transforms the news text to lowercase.
- The news text column of Bitcoin and Ethereum are passed to the master function to perform the above tasks and subsequently added to the respective sentiment scores dataframe.

### Section 3- Ngrams, WordCloud
- Tokenized lists containing the news article text for Bitcoin and Ethereum are created. All the content is transformed to a string.
- The top 10 bigrams and their freqency are determined and subsequently converted to a Dataframe.
- The WordCloud plot for Bitcoin and Ethereum are generated.

### Section 4- Named Entity recognition
- All the news article text is concatenated, one after the other, as a string.
- The NER visualization is rendered
- The entity names are listed.

## Difficulties encountered
This was the assignment for which I did the most amount of 'Googling'.
- Tokenizing the words in bitcoin_df['Text'] via a for-loop. A much simpler way of passing the tokenier function was taught by Khaled.
- Each word in the tokenized list was getting converted to a new row and column. Using list (zip...) fixed the problem. This was later found to be redundant.
- Concatenating all the news article text into a single object. With ','.join (map (str...), the obstacle was overcome.

## Conclusion/ My thoughts
- There is negligible amount of comparison involved in this project and it lacks a significant amount of quantitative analysis. Thus, I am unable to reach a conclusion on the task performed.
- In addition to the text analysis, another element about correlating the sentiment with the Bitcoin and Ethereum prices could have also been assigned. In my opinion, that would have been the appropriate 'Fintech' focused challenge.

## Contributors
- Satheesh Narasimman

## People who helped
- Khaled Karman, Bootcamp tutor

## References
- https://note.nkmk.me/en/python-pandas-list/

- https://datatofish.com/list-to-dataframe/

- https://towardsdatascience.com/from-dataframe-to-n-grams-e34e29df3460

- https://www.geeksforgeeks.org/python-iterate-through-value-lists-dictionary/

- https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.from_dict.html

- https://thispointer.com/pandas-create-dataframe-from-list-of-dictionaries/

- https://stackoverflow.com/questions/12453580/how-to-concatenate-items-in-a-list-to-a-single-string

- https://stackoverflow.com/questions/35864007/python-3-5-iterate-through-a-list-of-dictionaries

- https://stackoverflow.com/questions/38172097/convert-a-list-of-dictionaries-to-numpy-matrix

- https://stackoverflow.com/questions/36572221/how-to-find-ngram-frequency-of-a-column-in-a-pandas-dataframe
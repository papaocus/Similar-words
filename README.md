# Similar-words 
code begins by importing the necessary libraries, such as bs4 (BeautifulSoup), urllib, re, and nltk (Natural Language Toolkit).

It retrieves the content of a Wikipedia page on machine learning using the urllib.request.urlopen function and reads the HTML content.

The HTML content is parsed using BeautifulSoup to extract the paragraphs (<p>) from the page.

The paragraphs are then concatenated to form a single string of article text.

The script defines a class PreProcessText, which contains methods for removing punctuation and stopwords from the text.

The token_words method of the PreProcessText class removes punctuation and stopwords from the input text and returns a list of words.

The script checks if the stopwords from the nltk library are downloaded. If not, it attempts to download them.

If the stopwords are successfully downloaded, an instance of the PreProcessText class is created, and the token_words method is called on the article_text.

The script then imports Word2Vec from the gensim library.

It installs the gensim library using the pip install command.

Finally, the script initializes a Word2Vec model using the words list obtained from the preprocessing step.

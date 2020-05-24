# Text Data Analysis for CoMeDiAnS- NLP Project


## Install a Few Additional Packages

There are a few packages that are used - wordcloud, textblob and gensim.

## Summary:
Natural language processing (NLP) is an exciting branch of artificial intelligence (AI) that allows machines to break down and understand human language. This project includes text pre-processing techniques, machine learning techniques and Python libraries for NLP. 

Text pre-processing techniques include:

* tokenization
* text normalization
* data cleaning. 

## About the Project:

This is Natural Languaging project that involves:

### Web Scraping:

Web Scraping of a HTML web page to scrape the statements/dialogues/transacripts of all the comedians from "Scraps From The Loft". To decide which comedians to look into, I went on IMDB and looked specifically at comedy specials that were released in the past 5 years. To narrow it down further, I looked only at those with greater than a 7.5/10 rating and more than 2000 votes. If a comedian had multiple specials that fit those requirements, I would pick the most highly rated one. I ended up with a dozen comedy specials.

### Cleaning Data: 

It involves removal of punctuations, making text lowe case, removal of numerical values, remove numerical values, remove common non-sensical text (/n), Tokenize text and Remove stop words.

### Explore Data: 

In this process, I found out the most common words used by some specific comedian. I generated word clouds to have a visualization of the top 15 words that are used by the top comedian. This was done to get an idea of what makes that comedian the top one/ trending one? 

![image](https://user-images.githubusercontent.com/54689111/82752827-c852ae00-9d8e-11ea-80e2-8839572cd9b4.png)

I also figured out the number of unique words:

![image](https://user-images.githubusercontent.com/54689111/82752837-e1f3f580-9d8e-11ea-8e7b-156f9c9a855d.png)

I also figured out the bad words used:

![image](https://user-images.githubusercontent.com/54689111/82752856-018b1e00-9d8f-11ea-8e94-3c6711d8a2c0.png)


### Sentiment Analysis of the Comedian's transacripts:

When it comes to text data, there are a few popular techniques that we'll be going through in the next few notebooks, starting with sentiment analysis. A few key points to remember with sentiment analysis.

1. TextBlob Module: Linguistic researchers have labeled the sentiment of words based on their domain expertise. Sentiment of words can vary based on where it is in a sentence. The TextBlob module allows us to take advantage of these labels.

2. Sentiment Labels: Each word in a corpus is labeled in terms of polarity and subjectivity (there are more labels as well, but we're going to ignore them for now). A corpus' sentiment is the average of these.

* Polarity: How positive or negative a word is. -1 is very negative. +1 is very positive.

* Subjectivity: How subjective, or opinionated a word is. 0 is fact. +1 is very much an opinion.

### Topic Modelling:

The ultimate goal of topic modeling is to find various topics that are present in your corpus. Each document in the corpus will be made up of at least one topic, if not multiple topics.. In this project, I covered Latent Dirichlet Allocation (LDA), which is one of many topic modeling techniques. It was specifically designed for text data.

![image](https://user-images.githubusercontent.com/54689111/82752945-b8879980-9d8f-11ea-9935-f9b4cf60e1ae.png)

### Text Generation:

I used Markov chains for text generation. Think about every word in a corpus as a state. We can make a simple assumption that the next word is only dependent on the previous word - which is the basic assumption of a Markov chain. Below is a random text generated from a comedian : 'Ali Wong'

![image](https://user-images.githubusercontent.com/54689111/82752984-13b98c00-9d90-11ea-8780-f402037c51ad.png)

<h1 align="center">Bitcoin Price Prediction Using FNG and Closing Price Indicators</h1>
<h2 align="center"> A Deep Learning Project with Long Short-Term Memory Networks</h2>
<h4 align="center"> Created by <em>Cam Gould</em> for the <em>University of Toronto Fintech BootCamp</em> </h4>

<p align="center">
  <img
    src="https://github.com/CamGould/Natural_Language_Processing/blob/main/Supplemental/NLP_image.jpeg?raw=true"
  >
</p>

### Background Information
There's been a lot of hype in the news lately about cryptocurrency, making it quite challenging to distinguish between where public opinion lies.  That is why I set out to take stock, so to speak, of the latest news headlines and content regarding **Bitcoin** and **Ethereum** to get a better feel for the current public sentiment around each coin.
<br>
<br>
In this assignment, I will apply ***natural language processing*** to understand the sentiment in the latest news articles featuring *Bitcoin* and *Ethereum*. I will also apply *fundamental NLP techniques* to better understand the other factors involved with the coin prices such as common words and phrases and organizations and entities mentioned in the articles.
<br>
### Project Files
Use the following links to jump right into the anaylsis notebook or view results:
<br>
<br>
This notebook contains the [Natural Language Processing Techniques & Results](https://github.com/CamGould/Natural_Language_Processing/blob/main/Coding%20Notebooks/%5B1%5DCrypto_Sentiment.ipynb)
<br>
This image shows the [Numerical Sentiment Results for Bitcoin](https://github.com/CamGould/Natural_Language_Processing/blob/main/Supplemental/BTC_Results_NLP.png?raw=true)
<br>
This image shows the [Numerical Sentiment Results for Ethereum](https://github.com/CamGould/Natural_Language_Processing/blob/main/Supplemental/ETH_Results_NLP.png?raw=true)
<br>
### Project Outline and Instructions
#### Here is the structure of the [NLP Python Notebook](https://github.com/CamGould/Natural_Language_Processing/blob/main/Coding%20Notebooks/%5B1%5DCrypto_Sentiment.ipynb):
1. Sentiment Analysis 
    1. Here I use the [newsapi](https://newsapi.org/) to pull the latest news articles for Bitcoin and Ethereum and create a DataFrame of sentiment scores for each coin.
    2. I use this data to derive descriptive statistics to answer the following questions:
        1. Which coin had the *highest mean positive score*?
        2. Which coin had the *highest negative score*?
        3. Which coin had the *highest positive score*?
2. Natural Language Processing 
    1. In this section, I use *NLTK* and *Python* to tokenize text, find n-gram counts, and create word clouds for [Bitcoin](https://github.com/CamGould/Natural_Language_Processing/blob/main/Supplemental/BTC_word_cloud.png?raw=true) & [Ethereum](https://github.com/CamGould/Natural_Language_Processing/blob/main/Supplemental/ETH_Word_Cloud.png?raw=true). This involves:
        1. Lowercasing each word
        2. Removing all punctuation
        3. Removing all stopwords (Stop words are a set of commonly used words in any language that are considered unimportant in NLP)
3. Named Entity Recognition
    1. In this section, you will build a named entity recognition model for both coins and visualize the tags using SpaCy.

###  Key Findings and Visuals 
Here are the numerical findings for the sentiments on each coin.
<br>
<br>
Bitcoin - Descriptive Statistics:
<br>
![](https://github.com/CamGould/Natural_Language_Processing/blob/main/Supplemental/BTC_Results_NLP.png?raw=true)
<br>
<br>
Ethereum - Descriptive Statistics:
<br>
![](https://github.com/CamGould/Natural_Language_Processing/blob/main/Supplemental/ETH_Results_NLP.png?raw=true)
<br>
<br>
Here are the word clouds generated from each coins sentiment analysis.
<br>
<br>
Bitcoin - word cloud visual
<br>
![](https://github.com/CamGould/Natural_Language_Processing/blob/main/Supplemental/BTC_word_cloud.png?raw=true)
<br>
<br>
Ethereum - word cloud visual
<br>
![](https://github.com/CamGould/Natural_Language_Processing/blob/main/Supplemental/ETH_Word_Cloud.png?raw=true)

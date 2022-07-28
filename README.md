<h1 align="center">Bitcoin Price Prediction Using FNG and Closing Price Indicators</h1>
<h2 align="center"> A Deep Learning Project with Long Short-Term Memory Networks</h2>
<h4 align="center"> Created by <em>Cam Gould</em> for the <em>University of Toronto Fintech BootCamp</em> </h4>

<p align="center">
  <img
    src="https://github.com/CamGould/Deep_Learning_using_LSTM/blob/main/Supplemental/34084Bitcoin-Article-Cover-Image-3-scaled.jpg?raw=true"
  >
</p>

### Background Information
Due to the volatility of cryptocurrency speculation, investors will often try to incorporate sentiment from social media and news articles to help guide their trading strategies. One such indicator is the [Crypto Fear and Greed Index (FNG)](https://zipmex.com/learn/crypto-fear-and-greed-index-explained/) which attempts to use a variety of data sources to produce a daily FNG value for cryptocurrency. I will build and evaluate deep learning models using both the FNG values and simple closing prices to determine if the FNG indicator provides a better signal for cryptocurrencies than the normal closing price data.
<br>
<br>
In this assignment, I will use ***deep learning recurrent neural networks*** to model bitcoin closing prices. One model will use the *FNG indicators* to predict the closing price while the second model will use a *window of closing prices* to predict the nth closing price.
<br>
### Project Files
Use the following links to jump right into the anaylsis notebook or view results:
<br>
<br>
This notebook contains the [LSTM Stock Predictor from Closing Price](https://github.com/CamGould/Deep_Learning_using_LSTM/blob/main/Coding%20Notebooks/%5B1%5DLSTM_Stock_Predictor_Closing.ipynb)
<br>
This notebook contains the [LSTM Stock Predictor from FNG Indicators](https://github.com/CamGould/Deep_Learning_using_LSTM/blob/main/Coding%20Notebooks/%5B2%5DLSTM_Stock_Predictor_FNG.ipynb)
<br>
This graph shows the [price predictions for the closing price model](https://github.com/CamGould/Deep_Learning_using_LSTM/blob/main/Supplemental/Closing_graph.png)
<br>
This graph shows the [price predictions for the FNG model](https://github.com/CamGould/Deep_Learning_using_LSTM/blob/main/Supplemental/FNG_graph.png)
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

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
<br>
This graph shows the [price predictions for the closing price model](https://github.com/CamGould/Deep_Learning_using_LSTM/blob/main/Supplemental/Closing_graph.png)
<br>
This graph shows the [price predictions for the FNG model](https://github.com/CamGould/Deep_Learning_using_LSTM/blob/main/Supplemental/FNG_graph.png)
<br>
<br>
This file contains the [raw closing prices for BTC](https://github.com/CamGould/Deep_Learning_using_LSTM/blob/main/Supplemental/btc_historic.csv)
<br>
This file contains the [raw FNG indicators for BTC](https://github.com/CamGould/Deep_Learning_using_LSTM/blob/main/Supplemental/btc_sentiment.csv)

### Project Outline and Instructions
#### Prepare the Data for Training and Testing
1. Create a Jupyter Notebook for each RNN.
2. For the Fear and Greed model, use the FNG values to try and predict the closing price.
3. For the closing price model, use previous closing prices to try and predict the next closing price. 
4. Each model will need to use 70% of the data for training and 30% of the data for testing.
5. Apply a MinMaxScaler to the X and y values to scale the data for the model.
6. Reshape the X_train and X_test values to fit the model's requirement of samples, time steps, and features.

#### Build and Train LSTM RNNs
1. In each Jupyter Notebook, create the same custom LSTM RNN architecture. 
    1. In the first notebook, fit the data using the FNG values. 
    2. In the second notebook, fit the data using only closing prices.

###  Key Findings and Visuals 
#### Visual Price Predictions of Each Model:
***The Model using Closing Price*** - the far better performing model:
<br>
![](https://github.com/CamGould/Deep_Learning_using_LSTM/blob/main/Supplemental/Closing_graph.png?raw=true)
<br>
<br>
***The Model using FNG Indicators*** - a poor performing model:
<br>
![](https://github.com/CamGould/Deep_Learning_using_LSTM/blob/main/Supplemental/FNG_graph.png?raw=true)
<br>
<br>

#### Evaluating the Performance of Each Model

*Which model has a lower loss?*
<br> 

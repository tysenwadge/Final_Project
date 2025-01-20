# Forecasting Cryptocurrency Prices
### Forecasts made using Bloomberg's price data from 12/31/2019 - 1/6/2025
#### Using an LSTM machine model to predict the prices of Bitcoin, Ethereum, and SPY over the next 365 days
Slide Presentation: https://docs.google.com/presentation/d/1CC2Po0kCFion2GMhL2tDt-QxpxxH7qPPQLVvX-93Mws/edit

## For Github Readers: File Outline
- Typical Gitignore Files
- The main data file is named "Crypto_Data_2020_2025" in csv format
- This data was then separated into individual csvs for potential analysis: Bitcoin, Ethereum, Litecoin, Dogecoin, SPY (SP500 etf), CRP, and inflation data.
- We ran individual jupyter notebook files for Bitcoin, Ethereum, and SPY two times, one for training/testing and the other for predicting.
- There is a prediction graps folder which shows training/testing and forecasting for Bitcoin, Ethereum, and SPY.
- There is folder at the filepath: my_dir/bitcoin_lstm. This is where we created a crypto optimization models with Keras Tuner, equipped with epochs, training losses, and validation losses.

## Why we used an LSTM Model?
- LSTMs enable recurrent neural networks to recall inputs over a longer period of time
- Normalize the data
- Using a 60 day period lookback
- Training 75%, Testing 25%
- Forecasting Future  Prices for next 365 days
- RNNs are a robust and powerful type of neural network and are considered one of the most professional algorithms because they are the only ones with internal memory.
- Long short-term memory networks are an extension of recurrent neural networks, which basically extend the memory X_train and Y_train will be used to train the LSTM model, while X_test and Y_test will be used to evaluate its performance.

![BTC Training/Testing](https://github.com/ShaneRand/project-4/blob/main/prediction_graphs/bitcoin_prediction.png)


![BTC Forecasting](https://github.com/ShaneRand/project-4/blob/main/prediction_graphs/bitcoin_forecast.png)

![Ethereum Training/Testing](https://github.com/ShaneRand/project-4/blob/main/prediction_graphs/ethereum_prediction.png)


![Ethereum Forecasting](https://github.com/ShaneRand/project-4/blob/main/prediction_graphs/ethereum_forecast.png)

![SPY Training/Testing](https://github.com/ShaneRand/project-4/blob/main/prediction_graphs/spy_prediction.png)


![SPY Forecasting](https://github.com/ShaneRand/project-4/blob/main/prediction_graphs/spy_forecast.png)

## Which investment to make?
That depends on your appetite for risk. If you trust the model and can buy BTC or Ethereum at less than the forecasted price, and can accept the riskiness of cryptocurrency, the returns since 2019 are great. Safer assets like SPY (index fund on SP500) or Fidelity's mutual fund, provide adequate returns over the same horizon.

## Assumptions and Limitations
- LSTM models are susceptible to overfitting. 
- LSTMs are often known as "black-box" models, making it difficult to analyze how one arrives at particular decisions.
- LSTMs on larger data sets can be very time intensive.
- Complexity: LSTMs have a more sophisticated architecture compared to other RNNs or feedforward neural networks. This complexity can make them more challenging to implement and tune.

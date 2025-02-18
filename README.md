# 5th-sem-ML-Project
This project implements a stock price prediction model using LSTM (Long Short-Term Memory) neural networks. It utilizes historical stock price data from Yahoo Finance, preprocesses it using MinMax scaling, and trains a deep learning model to predict future stock prices. The model is then evaluated by comparing predicted prices with actual prices.

Stock Price Prediction using LSTM
Overview

This project predicts stock prices using a Long Short-Term Memory (LSTM) model. It fetches stock data from Yahoo Finance, preprocesses it, and trains an LSTM network using TensorFlow/Keras to predict future price trends.
Features

    Fetches historical stock price data via Yahoo Finance API
    Implements moving average analysis (100-day & 200-day)
    Preprocesses data with MinMaxScaler
    Builds a 4-layer LSTM model with dropout regularization
    Trains and tests the model using 80-20% split
    Visualizes predictions vs actual stock prices
    Saves the trained model for future use

Requirements

    Python 3.x
    NumPy
    Pandas
    Matplotlib
    Scikit-learn
    TensorFlow/Keras
    yFinance

Usage

    Install dependencies using:

pip install numpy pandas matplotlib scikit-learn tensorflow yfinance

Run the script:

    python stock_prediction.py

    The model will train and plot actual vs predicted prices.

Model Training Details

    Input: 100 days of past stock prices
    Architecture: 4 LSTM layers with dropout
    Optimizer: Adam
    Loss Function: Mean Squared Error (MSE)
    Epochs: 50
    Batch Size: 32

Output

    The model saves as Stock Predictions Model.keras
    Generates a visualization of actual vs predicted prices

Future Improvements

    Implement real-time stock prediction
    Use different stock indicators (RSI, MACD)
    Experiment with transformer-based models

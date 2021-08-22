# SimpleTimeSeriesLSTM
📉 Simple LSTM network for analyzing financial time-series

## About The Project
LSTM is a type of neural network that excels at processing data with sequential dependencies, making it an ideal candidate for analyzing time series financial data.
This repo contains a simple example of using LSTM to predict the next day's price of bitcoin. It performs surprisingly well. 

## How To Run
The easiest way to run this project is to download the Jupyter notebook with the example on GitHub. Since the project uses Python, the best way to run it is through Jupyter notebooks, which are accessible from any program that can read and write JSON files (such as IDLE or Notebook). 
Alternatively, you can run the code in colab. 
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14GRudIH3j-SmTvd41VG1t_kmvdyQJNXZ)

# Challenges
The Program used MinMaxScaler which when given a feature range of [0,1], the predictions would blow out of proportions. ***Probably running out of floating point space. *** Problem was solved with by widening the feature range to [0,5]. 

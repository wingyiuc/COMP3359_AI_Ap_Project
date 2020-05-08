# Cryptocurrency Trading using LSTM
This project contains the code for the *Cryptocurrency Trading using LSTM* project. It trains on historical cryptocurrencies price and technical indicators data, and presents the backtesting performance.
## Getting Started
### Prerequisites
The project requires python libraries: `os`, `pandas`, `numpy`, `datetime`, `glob`, `requests`, `matplotlib`, `math`, `ta` (for technical analysis), `pywt` (for wavelet transform), `tensorflow`, `keras`, `sklearn`, `seaborn` and `random`.
## Walk_forward_Models_(Final).ipynb
### 0. Getting started
1. Change your file path on `module_dir`. 
2. Install and load packages. 
3. Run all the **Global variables & functions**.
### Walkforward Model with Online Learning: LSTM & CNN on Bitcoin
This section gives walk-forward model with online-learning on any specified crypto ticker. It outputs the total accuracy, accuracy confusion matrix and profit & loss graph. 
### Transfer learning from other cryptos
This section gives transfer learning model that learns from all other crypto, and apply on BTC.
### LSTM General performance on all cryptos
This section provides the accuracy confusion matrix on the LSTM out-of-sample accuracy of *all* cryptos in the tickers list. 
### CNN General Performance on All Cryptos
This section provides the accuracy confusion matrix on the CNN out-of-sample accuracy of *all* cryptos in the tickers list.

## LSTM_1_Day_Regression_Presentation
This folder correspinding to Section 5: LSTM Regression 1-day Return. 

### ARMA(3,5) Model: The predictions produced by the basemodel ARMA(3,5)
  - ARMA(3,5) Return Prediction Only Compatible with LSTM.ipynb: Implement ARMA(3,5) 

### LSTM 1day Return Dropout 0.02 LeakyReLu: Implementation of LSTM models using the dropout rate = 0.02
  - LSTM1.ipynb: Implement LSTM1
  - LSTM2.ipynb: Implement LSTM2
  - LSTM3.ipynb: Implement LSTM3
  - LSTM4.ipynb: Implement LSTM4
    - The defintiions of LSTM1 to LSTM4 can be found in the final report.
  - Result_ARMA_LSTM_Evaluation.ipynb: Comparing the results produced by LSTM models with the ARMA(3,5) model
### LSTM 1day Return Dropout 0.2 LeakyReLu: Implementation of LSTM models using the dropout rate = 0.2
  - LSTM1.ipynb: Implement LSTM1
  - LSTM2.ipynb: Implement LSTM2
  - LSTM3.ipynb: Implement LSTM3
  - LSTM4.ipynb: Implement LSTM4
    - The defintiions of LSTM1 to LSTM4 can be found in the final report.
  - Result_ARMA_LSTM_Evaluation.ipynb: Comparing the results produced by LSTM models with the ARMA(3,5) model

## Time_Series_Model_Presentation
This folder corresponding to Section 3.2.: Time Series Characteristics of BTC
- Time Series Characteristics of BTC.ipynb: Time Seris Anlaysis of BTC close price

## CNN_transfer_learning
This folder corresponding to Section 7.3: Discussion. It only perform the transfer learning using FX and Commodity data
- CNN_Prepare_Data_CNN_transfer_learning_using_FX_Commo.ipynb: This notebook prepares the H5files of FX and Commodity for CNN_transfer_learning_using_FX_Commo.ipynb
- CNN_Prepare_Data.ipynb: This notebook prepares the H5files of BTC for CNN_transfer_learning_using_FX_Commo.ipynb
- CNN_transfer_learning_using_FX_Commo.ipynb: This notebook implements the CNN transfer learning model
- Data_Handling_CNN_transfer_learning_using_FX_Commo.ipynb: This notebook preprocesses the raw data of FX and Commodity 
- Data_Handling_CNN_transfer_learning_using_FX_Commo.ipynb: This notebook preprocesses the raw data of BTC

## 'Cryptocurrency data' file
All the raw data that contains historical prices and volumes are under the *Raw data* subdirectory under *Cryptocurrency data*. To produce technical indicators, run the `Data_processing_(Final).ipynb`, which would generate csv files with technical indicators and truth labels. All files are saved in *Processed data* subdirectory under *Cryptocurrency data*. 

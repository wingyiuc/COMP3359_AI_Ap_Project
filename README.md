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
## 'Cryptocurrency data' file
All the raw data that contains historical prices and volumes are under the *Raw data* subdirectory under *Cryptocurrency data*. To produce technical indicators, run the `Data_processing_(Final).ipynb`, which would generate csv files with technical indicators and truth labels. All files are saved in *Processed data* subdirectory under *Cryptocurrency data*. 

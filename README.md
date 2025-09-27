Stock Price Prediction Using LSTM
Project Overview
This project demonstrates time-series forecasting for Microsoft (MSFT) stock prices from January 2020 to September 2025 using a PyTorch-based LSTM neural network. The notebook covers all stages: data acquisition, processing, model building, training, evaluation, and visualization.

Features
Comprehensive Data Pipeline: Automates data download, preprocessing, and windowing for time-series analysis using pandas, numpy, and sklearn.

Custom LSTM Model: Implements a multi-layer neural network in PyTorch for predicting future stock prices from historical trends.

Training and Evaluation: Optimizes the model using Adam, tracks RMSE (Root Mean Square Error) for accuracy, and compares prediction errors visually.

Visualization: Provides informative plots: actual vs predicted stock prices and error trends throughout the test period.

Installation & Usage
Prerequisites
Python 3.7+

Jupyter Notebook

Recommended packages: numpy, pandas, matplotlib, torch, scikit-learn, yfinance

Steps to Run
Clone or Download: Save main.ipynb and ensure all dependencies are installed.

Edit Ticker (optional): By default, the ticker symbol is set to 'MSFT'. For other stocks, replace 'MSFT' in code cells accordingly.

Run Notebook: Execute each cell sequentially to download data, preprocess, train, and visualize results.

Modify Model (optional): Adjust hyperparameters (hidden layers, sequence length, epochs) in designated cells to improve performance or experiment.

Example Command
python
# To install dependencies
pip install numpy pandas matplotlib torch scikit-learn yfinance
Repository Structure
Section	Purpose
Data Acquisition	Download and clean MSFT stock data using yfinance
Preprocessing	Normalize and window historical closing prices
Model Architecture	Define and initialize PyTorch LSTM-based prediction class
Training Loop	Fit model, output loss and accuracy metrics (RMSE)
Evaluation	Plot actual vs predicted prices, visualize error trends
Error Analysis	Notes on common errors and troubleshooting (markdown cells)
Customization	Hyperparameter tuning, alternative tickers (user-editable cells)
Key Results
Performance Metrics: Reports train RMSE and test RMSE after each run.

Visual Insights: Plots show time-series comparison and error distributions for easy analysis.

Troubleshooting
Column Selection Error: If errors relating to DataFrame column selection occur, check if columns are referenced by tuple (df['Close', 'MSFT']) instead of attribute (df.Close).

Hardware: GPU detection is coded; if unavailable, defaults to CPU seamlessly.

License
This project is for educational and research purposes.

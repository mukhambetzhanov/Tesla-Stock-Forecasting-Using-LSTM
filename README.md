# Tesla-Stock-Forecasting-Using-LSTM
## Tesla Stock Price Forecasting with Long Short-Term Memory (LSTM) Neural Network

Welcome to my GitHub repository for the project "Tesla Stock Price Forecasting with Long Short-Term Memory (LSTM) Neural Network." In this project, I have developed an LSTM-based neural network to predict the future closing prices of Tesla (TSLA) stock. The primary goal of this project is to showcase the implementation of a time series forecasting model using PyTorch and deep learning techniques.

### Project Overview:
In this project, I have performed the following tasks:

1. **Data Preparation:**
   - Loaded historical Tesla stock price data from a CSV file obtained from Yahoo Finance.
   - Preprocessed the data by subsetting the 'Date' and 'Close' columns and converting the 'Date' column to datetime format.
   - Created a custom function to transform the dataset into a suitable format for LSTM input by incorporating past closing prices as features.

2. **Data Preprocessing:**
   - Normalized the data using Min-Max scaling to ensure that it lies within a specific range for better model convergence.

3. **Model Architecture:**
   - Designed a custom LSTM neural network model using PyTorch's `nn.Module` class.
   - The LSTM model takes a sequence of past closing prices as input and predicts the next closing price.

4. **Training and Validation:**
   - Utilized PyTorch's `DataLoader` to efficiently load and process training and validation data in mini-batches.
   - Implemented training and validation loops to train the LSTM model on historical data while monitoring the loss function.
   - Utilized Mean Squared Error (MSE) loss as the optimization criterion.

5. **Evaluation and Visualization:**
   - Evaluated the model's performance on both training and testing data.
   - Generated predictions for the closing prices of both training and testing data and inversely transformed them to the original scale.
   - Visualized the actual vs. predicted closing prices over time using Matplotlib.

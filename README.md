# Realtime-Stock-Prediction
Stock Trend Prediction Web Application in Python using Streamlit, an open-source Python library, that makes it easy to build beautiful custom web apps for Machine Learning and Data Science.
Methodology:
1. Import necessary libraries: Import the required libraries such as numpy, pandas, matplotlib, keras, streamlit, pandas_datareader, and yfinance.
2. Set start and end dates: Define the start and end dates for retrieving stock data.
3. Set up Streamlit interface: Create a Streamlit application with a title and a text input field to allow the user to enter a stock ticker.
4. Retrieve stock data: Use the Yahoo Finance API to fetch the historical stock data for the specified stock ticker and time period.
5. Describe the data: Display the statistical summary of the retrieved data using the describe() function.
6. Visualize the data: Create and display two line charts using matplotlib. The first chart shows the closing price of the stock over time, and the second chart shows the closing price along with a 100-day moving average.

7. Prepare the training data: Split the data into training and testing sets. Take 70% of the data for training. Normalize the training data using MinMaxScaler.

8. Build the model: Load a pre-trained Keras model from a specified file path.

9. Prepare the testing data: Take the last 100 days of the training data and append it with the testing data. Normalize the combined data using the same scaler used for training.

10. Perform predictions: Use the model to predict the stock prices for the test data. Rescale the predicted and original prices to their original scale using the scaler.

11. Display predictions: Create a line chart to compare the predicted and original prices of the stock.

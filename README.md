**Stock Market Price Prediction using Stacked LSTM**

This project predicts the stock market price for the next 30 days using a stacked Long Short-Term Memory (LSTM) model. The model is trained on historical stock prices fetched using the pandas_datareader library, and the predictions are made for Google’s stock price (ticker: GOOG). The data is preprocessed using scaling techniques and split into training and test datasets to develop an accurate forecasting model.

**Features**

	•	Uses historical stock price data from Tiingo API.
	•	Implements a stacked LSTM model for time series prediction.
	•	Predicts stock prices for the next 30 days.
	•	Data visualization of the stock trends.

**Prerequisites**

The following Python packages are required to run the project:

	•	pandas==1.5.3
	•	pandas_datareader==0.10.0
	•	matplotlib
	•	scikit-learn
	•	tensorflow
	•	keras

To install the required packages, use the following command:

pip install -r requirements.txt

**Datasets**

The stock data is fetched using the Tiingo API for the stock ticker GOOG (Google). The data is then saved to a CSV file for further processing and analysis.

**Usage**

1. Clone this repository:

   https://github.com/naman1824/Stock-Market-Analysis-Using-Deep-Learning

2. Setup the environment by installing depenedencies:

   pip install -r requirements.txt

3. Download the stock price data using the Tiingo API(make sure you have an API key):

   df = pdr.get_data_tiingo('GOOG', api_key='your_api_key_here')
   df.to_csv('GOOG.csv')

4. Preprocess the data by normalizing and splitting it into training and testing sets.

5. Build and train the stacked LSTM model as described in the script:

   from tensorflow.keras.models import Sequential
   from tensorflow.keras.layers import LSTM, Dense

6. Use the trained model to predict the stock prices for the next 30 days.
	
7. Plot the results to visualize the predictions:

   plt.plot(predictions)
   plt.show()

**File Structure**

	•	stockmarketdl.py: The main Python script that performs data fetching, preprocessing, model training, and prediction.

 **License**

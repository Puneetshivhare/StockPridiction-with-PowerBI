
# Stock Price Prediction using LSTM with Power BI Dashboard

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Approach](#approach)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Power BI Dashboard](#power-bi-dashboard)
- [Challenges and Improvements](#challenges-and-improvements)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
This project involves building a Long Short-Term Memory (LSTM) based machine learning model to predict stock prices. The focus is on achieving a good prediction accuracy and presenting the results on a **Power BI** dashboard. The dashboard provides a dynamic and user-friendly interface to visualize stock market trends, news, and technical indicators.

**Key Features:**
- Developed using an **LSTM neural network**.
- Data preprocessed through **Exploratory Data Analysis (EDA)** and feature engineering.
- **Power BI Dashboard** for dynamic visualization of stock trends, technical indicators, and news sentiment.

## Dataset
The dataset used in this project includes historical stock prices, with attributes such as:
- Open, High, Low, Close, Adjusted Close prices.
- Trading Volume.
- Additional features created through **feature engineering**.

sourced stock price data from publicly available APIs like Yahoo Finance. Additionally.

## Approach
1. **Data Collection & Cleaning**: Acquired historical stock data and cleaned it by handling missing values, removing outliers, and standardizing formats.
2. **Exploratory Data Analysis (EDA)**: Identified key patterns and trends, and selected essential features.
3. **Model Building**: Developed a LSTM-based neural network for time series forecasting using **TensorFlow**/ **Keras**.
4. **Training & Evaluation**: Trained the model and achieved an accuracy of around **47%**.
5. **Power BI Integration**: Created an interactive dashboard to showcase predicted stock trends, actual stock prices, news sentiment, and technical indicators.

## Project Structure
```
Stock-Prediction-LSTM-PowerBI/
│
├── data/
│   ├── stock_data.csv                 # Stock price dataset
│
├── notebooks/
│   ├── data_cleaning.ipynb            # Data cleaning and preparation
│   ├── feature_engineering.ipynb      # Feature engineering notebook
│   ├── LSTM_model.ipynb               # Model training and evaluation
│
├── src/
│   ├── data_processing.py             # Data processing functions
│   ├── feature_generation.py          # Feature generation functions
│   ├── model.py                       # LSTM model definition
│   ├── train.py                       # Script to train the model
│
├── dashboard/
│   ├── stock_dashboard.pbix           # Power BI dashboard file
│
├── README.md                          # Project documentation
└── requirements.txt                   # Python package requirements
```

## Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/username/Stock-Prediction-LSTM-PowerBI.git
   cd Stock-Prediction-LSTM-PowerBI
   ```

2. **Install Required Packages**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Download Power BI**:
   - [Download Power BI Desktop](https://powerbi.microsoft.com/desktop/) and install it on your system to access the dashboard.

## Usage
1. **Prepare the Dataset**:
   Place your historical stock price dataset (`stock_data.csv`) in the `data/` folder.

2. **Run the Data Processing & Feature Engineering**:
   ```bash
   python src/data_processing.py
   python src/feature_generation.py
   ```

3. **Train the LSTM Model**:
   ```bash
   python src/train.py
   ```

4. **Evaluate the Model**:
   Analyze the results in the model training notebook or using scripts.

5. **Load Power BI Dashboard**:
   - Open the `dashboard/stock_dashboard.pbix` file using Power BI Desktop.
   - Update the data source if required to reflect the latest stock data.

## Results
The LSTM model achieved a stock price prediction accuracy of **47%**. The **Power BI dashboard** was used to create an interactive experience with the following features:
- **Stock Trends**: A comparison between actual and predicted stock prices.
- **Technical Indicators**: Display of moving averages, RSI, etc.
- **News Sentiment**: An integration of sentiment analysis results from Twitter or Reddit.

## Power BI Dashboard
The Power BI dashboard is designed to provide:
- **Visual Charts** for stock prices and predictions.
- **Interactive Controls** to filter by date ranges and other parameters.
- ![image](https://github.com/user-attachments/assets/7ed7855b-dec8-43dd-8398-e24cb3c341ba)


## Challenges and Improvements
- **Challenges**: The prediction accuracy was limited to **47%**, mainly due to stock market volatility and insufficient sentiment data.
- **Improvements**: Potential improvements include:
  - Incorporating additional technical and economic indicators.
  - Refining the model with more advanced architectures (e.g., GRU or attention-based networks).
  - Enhancing the sentiment analysis with additional sources.

## Contributing
If you'd like to contribute, feel free to fork this repository and submit a pull request with your changes.

## License
This project is licensed under the **MIT License**.

---

Feel free to customize it based on your preferences or add more details relevant to your project.

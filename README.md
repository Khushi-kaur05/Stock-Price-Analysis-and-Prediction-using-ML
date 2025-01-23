# Stock Price Prediction Using LSTM

This project is a comprehensive implementation of stock price prediction using Long Short-Term Memory (LSTM) neural networks. It involves data collection, preprocessing, feature engineering, model building, and evaluation. The project focuses on analyzing stock market trends and predicting future prices based on historical data.

---

## Features of the Project

- **Data Collection:**
  - Historical stock data is fetched using the `yfinance` library.
  - Data includes Adjusted Close price, Volume, and other features.

- **Data Preprocessing:**
  - Missing values are handled appropriately.
  - New features like Moving Averages (20-day and 50-day) are added.
  - Data is scaled using Min-Max scaling for better performance during model training.

- **Exploratory Data Analysis (EDA):**
  - Plots of Adjusted Close prices and Moving Averages for trend analysis.
  - Volume analysis to understand trading activity and more.

- **Model Building:**
  - LSTM model is built using TensorFlow/Keras with the following architecture:
    - Two LSTM layers with 50 units each.
    - Dropout layers to prevent overfitting.
    - Dense layer to output the predicted price.
  - Optimizer: Adam
  - Loss Function: Mean Squared Error (MSE)

- **Cross-Validation:**
  - 5-fold cross-validation is performed to evaluate the model.

- **Training and Testing:**
  - The data is split into training and testing sets based on an 80-20 ratio.
  - Each stock (ticker) is trained separately to generate specific models.

- **Evaluation:**
  - The model is evaluated using Mean Absolute Error (MAE) and testing accuracy.
  - Actual vs. Predicted prices are plotted for visual comparison.

- **Results Storage:**
  - Predictions and actual values are saved in CSV files for further analysis.

---

## Technologies and Libraries Used

- **Programming Language:** Python
- **Libraries:**
  - `yfinance` for data collection.
  - `pandas` and `numpy` for data manipulation.
  - `matplotlib` for data visualization.
  - `scikit-learn` for data scaling and evaluation metrics.
  - `tensorflow`/`keras` for building and training the LSTM model.





---

## Acknowledgments

Special thanks to the open-source community for tools and resources like `yfinance`, `TensorFlow`, and `scikit-learn`, which made this project possible.


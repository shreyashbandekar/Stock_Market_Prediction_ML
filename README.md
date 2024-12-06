 # ***Stock Market Prediction Model***
## **Overview**
This repository contains a comprehensive project for predicting stock market trends using historical stock data. The project leverages Python for data acquisition, analysis, and machine learning model creation. The primary goal is forecasting stock prices and providing insights into market movements.

### **Features**
* **Data Acquisition:** Fetches historical stock data using [Yahoo Finance](https://finance.yahoo.com/).
* **Data Visualization:** Visualizes trends and patterns in stock prices.
* **Predictive Modeling:** Implements machine learning models to predict future stock prices.
* **Modular Code Structure:** Clean and modular code for better readability and extensibility.


### **Technologies Used**
* Programming Language: Python 3.12.5
* **Libraries:**
  * `numpy` and `pandas` for data manipulation
  * `matplotlib` for data visualization
  * `yfinance` for stock data acquisition

### **Installation**

#### 1. Clone the repository:
```
git clone https://github.com/shreyashbandekar/Stock-Market-Prediction-Model.git
cd Stock-Market-Prediction-Model
```
#### 2. Install required dependencies:
```
pip install -r requirements.txt
```
#### 3. Ensure you have installed Python 3.12 or higher.
-----
## **How to Use**
#### 1. Run the Notebook:
 - Open the Jupyter Notebook file `Stock_Market_Prediction_Model_Creation.ipynb`.
 - Follow the cells in sequence to fetch stock data, preprocess it, and train the model.

#### 2. Load the Model:
 - Use the pre-trained model provided (`Stock Predictions Model.keras`) or train your own using the notebook.
 - To make predictions, load the model in Python:
```python
from tensorflow.keras.models import load_model
model = load_model('Stock Predictions Model.keras')
```
#### 3. Visualize Results:

- Utilize the included plots and visualizations to analyze model predictions against actual data.
---


## **Example**

Here is an example of fetching Google’s stock data and visualizing it:

```python
import yfinance as yf
import matplotlib.pyplot as plt

start = '2012-01-01'
end = '2024-12-21'
stock = 'GOOG'

data = yf.download(stock, start, end)
data['Close'].plot(title=f"{stock} Stock Prices", figsize=(10, 6))
plt.show()
```


## **Acknowledgments**

- [Yahoo Finance](https://finance.yahoo.com/) for stock data.

- [TensorFlow](https://www.tensorflow.org/) for model building.

-----
**Happy Predicting! 🚀**

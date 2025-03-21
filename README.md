# Foundation-model-Water-Level-Forecasting-
This repository contains a Python implementation for water level forecasting using the TimesFM model. The model performs a rolling forecast to predict water levels at a given gauge location for three days ahead. The code is organized into multiple sections for loading data, training the model, forecasting, and evaluating the results.

---



## Sections

1. **Install Required Libraries and Import Modules**  
   Installs the necessary libraries and imports the required Python modules for data manipulation, machine learning, and visualization.
2. **Data Loading and Preprocessing**  
   Loads the water discharge data from a CSV file, preprocesses the data by handling missing values, and prepares the dataset for time series forecasting.

3. **Time Series Data Splitting and Visualization**  
   Splits the dataset into training, validation, and test sets. Visualizes the water levels over time and highlights the training, validation, and test periods.

4. **Initialize TimesFM Model**  
   Initializes the TimesFM model with pretrained weights and sets the necessary hyperparameters for forecasting.

5. **Rolling Forecast Using TimesFM**  
   Performs a rolling forecast on the water level data using the TimesFM model, predicting three days ahead for each rolling window.

6. **Processing Forecast Results**  
   Processes the forecast results to shift and align the predicted values with the actual observed values.

7. **Visualization of Forecast vs Observed Data**  
   Visualizes the forecasted values (for Day 1, Day 2, and Day 3) against the observed water levels to assess the model’s performance.

8. **Model Evaluation - Nash-Sutcliffe and Kling-Gupta Efficiency**  
   Evaluates the model performance using two common evaluation metrics: Nash-Sutcliffe Efficiency (NSE) and Kling-Gupta Efficiency (KGE).

---



## Requirements

To run this code, you will need the following libraries:

- `timesfm`
- `tensorflow`
- `pandas`
- `numpy`
- `matplotlib`
- `google.colab`

You can install the required libraries by running the following commands:


`!pip install timesfm'`

---



##Usage
1. Clone the repository:
`git clone https://github.com/your-username/water-level-forecasting.git`


2. Upload your dataset to Google Drive and update the path to the dataset in the script:

`data_file = '/content/drive/MyDrive/germany_gauges/CAMELS_DE_discharge_sim_DE214640.csv'`


3. Run the script on Google Colab to perform time series forecasting:

*   Load and preprocess the data.
*   Train the TimesFM model on the training data.
*   Perform a rolling forecast on the test data.
*   Visualize and evaluate the results.

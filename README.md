# IoT Household Energy Consumption Analysis and Forecasting

This project demonstrates skills in using, analyzing, and visualizing IoT data from a household energy consumption dataset. It includes data cleaning, exploratory data analysis (EDA), visualization using Power BI, and machine learning for electricity load forecasting.

## Dataset Description

The dataset contains 2,075,259 measurements gathered in a house located in Sceaux (7km from Paris, France) between December 2006 and November 2010 (47 months). The data includes various energy consumption metrics and is in CSV format.

### Data Fields:
1. **date**: Date in format dd/mm/yyyy
2. **time**: Time in format hh:mm:ss
3. **global_active_power**: Household global minute-averaged active power (in kilowatt)
4. **global_reactive_power**: Household global minute-averaged reactive power (in kilowatt)
5. **voltage**: Minute-averaged voltage (in volt)
6. **global_intensity**: Household global minute-averaged current intensity (in ampere)
7. **sub_metering_1**: Energy sub-metering No. 1 (in watt-hour of active energy). It corresponds to the kitchen, containing mainly a dishwasher, an oven, and a microwave (hot plates are not electric but gas powered).
8. **sub_metering_2**: Energy sub-metering No. 2 (in watt-hour of active energy). It corresponds to the laundry room, containing a washing-machine, a tumble-drier, a refrigerator, and a light.
9. **sub_metering_3**: Energy sub-metering No. 3 (in watt-hour of active energy). It corresponds to an electric water-heater and an air-conditioner.

## Project Goals

1. **Data Cleaning and Wrangling**: Prepare the dataset for analysis by handling missing values and converting data types.
2. **Exploratory Data Analysis (EDA)**: Gain insights into the energy consumption patterns and relationships between variables.
3. **Visualization**: Create informative visualizations using Power BI to showcase the data.
4. **Machine Learning**: Develop a model to forecast electricity load based on historical data.

## Project Structure

```
project-root/
├── data/
│   └── household_energy_consumption.csv
├── notebooks/
│   ├── 01_data_cleaning_and_wrangling.ipynb
│   ├── 02_exploratory_data_analysis.ipynb
│   └── 03_machine_learning.ipynb
├── powerbi/
│   └── household_energy_dashboard.pbix
├── src/
│   └── utils.py
├── README.md
└── requirements.txt
```

## Step-by-Step Guide

### 1. Data Cleaning and Wrangling

**File:** `notebooks/01_data_cleaning_and_wrangling.ipynb`

- **Load the Data**: Use pandas to read the CSV file.
- **Handle Missing Values**: The dataset has about 1.25% missing values. Replace missing values with appropriate methods (e.g., mean imputation for numerical columns).
- **Convert Data Types**: Convert `date` and `time` columns to datetime format. Convert other columns to appropriate numeric types.
- **Create New Features**: Calculate total energy consumption and create time-based features (e.g., day of week, month, year).
- **Save Cleaned Data**: Save the cleaned dataset for further analysis.


### 2. Exploratory Data Analysis (EDA)  
**File:** `notebooks/02_exploratory_data_analysis.ipynb`  

 
- **Descriptive Statistics**: Calculate and visualize basic statistics for each variable.  
- **Time Series Analysiss**: Analyze trends and seasonality in energy consumption over time.  
- **Correlation Analysis**: Examine relationships between different energy consumption metrics.  
- **Distribution Analysis**: Visualize the distribution of key variables.

### 3. Visualization with Power BI  
**File:** `powerbi/household_energy_dashboard.pbix`  

### Import Data  
- Load the cleaned dataset into Power BI.  

### Create Visualizations  
- Line chart for global active power over time.  
- Bar chart for average energy consumption by month.  
- Pie chart for energy distribution across sub-meterings.  
- Scatter plot to show the relationship between voltage and global intensity.  
- Interactive filters for date range and specific metrics.  

### Dashboard Layout  
- Arrange visualizations in a coherent and informative layout.  

### Insights  
- Add text boxes to highlight key findings and insights from the data.
### 4. Machine Learning for Electricity Load Forecasting  
**File:** `notebooks/03_machine_learning.ipynb`  

#### Data Preparation  
- Prepare the data for time series forecasting, including feature engineering and splitting into train/test sets.  

#### Model Selection  
- Choose an appropriate model for time series forecasting (e.g., ARIMA, LSTM, or Prophet).  

#### Model Training  
- Train the selected model on the training data.  

#### Model Evaluation  
- Evaluate the model's performance using appropriate metrics (e.g., MAE, RMSE).  

#### Forecasting  
- Use the trained model to forecast future electricity load.

## Conclusion
In this project, we analyzed a comprehensive dataset of household energy consumption collected over 47 months in Sceaux, France. Through our data cleaning and wrangling efforts, we prepared the dataset for in-depth analysis, handling missing values creating features to enhance our understanding of energy usage patterns. Our exploratory data analysis (EDA) provided valuable insights into the distribution, trends, and relationships within the, revealing daily, monthly, and yearly patterns in energy consumption.

We utilized Power BI to create an interactive dashboard, visualizing key metrics such as global active power over time, average energy consumption by month, energy distribution across different sub-meterings, and the relationship between voltage and global intensity. This dashboard not only an easier interpretation of the data but also allowed for real-time exploration of different time periods and metrics.

Furthermore, we implemented a machine learning model using ARIMA for electricity load forecasting. While the initial model produced a straight-line forecast, further tuning and exploration of other models like SARIMA or even advanced techniques such as LSTM could potentially yield more nuanced predictions. The project demonstrated the power of combining data analysis, visualization, and predictive modeling to gain actionable insights from IoT data, which can be invaluable for optimizing energy usage and planning in household settings.


## Future Work  

### Advanced Machine Learning  
- Explore more advanced models like LSTM or Prophet for improved forecasting accuracy.  

### Real-time Monitoring  
- Implement a real-time monitoring system using the IoT data.  

### Energy Efficiency Recommendations  
- Develop a system to provide personalized energy-saving recommendations based on the analysis.  

## Requirements
To run the notebooks, you'll need the following Python libraries:
```
pandas
numpy
matplotlib
seaborn
statsmodels
scikit-learn ```

You can install them using:
``` pip install -r requirements.txt ```


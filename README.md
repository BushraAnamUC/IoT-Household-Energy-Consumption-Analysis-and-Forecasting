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
,,,
project-root/
├── data/
│ └── household_energy_consumption.csv
├── notebooks/
│ ├── 01_data_cleaning_and_wrangling.ipynb
│ ├── 02_exploratory_data_analysis.ipynb
│ └── 03_machine_learning.ipynb
├── powerbi/
│ └── household_energy_dashboard.pbix
├── src/
│ └── utils.py
├── README.md
└── requirements.txt
,,,

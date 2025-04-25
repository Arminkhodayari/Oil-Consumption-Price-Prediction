# Oil-Consumption-Price-Prediction
This project analyzes global oil consumption and predicts oil prices using historical datasets. Key features of the project include:

Data Cleaning & Transformation : Converting raw datasets into a structured format.
Exploratory Data Analysis (EDA) : Visualizing trends in oil prices, GDP, inflation, and other variables over time.
Forecasting Models :
ARIMA Model : Predicts oil prices based on GDP as an exogenous variable.
LSTM Neural Network : Provides nonlinear forecasts for oil prices with adjustments for future scenarios.
Scenario Analysis : Compares two scenarios—current trajectory (with geopolitical shocks) and net-zero pledges—to predict long-term oil price trends.
Table of Contents
Files Included
Dependencies
How to Run
Analysis Highlights
Forecasting Results
Contributions
Files Included
All files are located in the root directory of the repository:

brent-year.csv : Historical Brent crude oil price data (yearly).
crude-oil-exports.CSV : Annual crude oil export volumes (in million cubic meters).
crude-oil-imports.CSV : Annual crude oil import volumes (in million cubic meters).
crude-oil-production.CSV : Annual crude oil production data (in million cubic meters).
GDP.CSV : Global GDP data (current US$).
oil-consumption WORLD.CSV : Global oil consumption data (TWh).
Inflation.csv : Global inflation rates from 1981 to 2023.
Untitled4.ipynb : The main Jupyter Notebook containing the analysis and forecasting code.
combined_data.csv : Processed dataset combining all raw datasets.
Dependencies
The following Python libraries are required to run the project:

bash
Copy
1
2
3
4
5
6
7
pandas
numpy
matplotlib
seaborn
statsmodels
tensorflow
sklearn
You can install all dependencies using the requirements.txt file (if available):

bash
Copy
1
pip install -r requirements.txt
How to Run
Clone the Repository :
bash
Copy
1
2
git clone https://github.com/your-username/Oil-Consumption-Price-Prediction.git
cd Oil-Consumption-Price-Prediction
Install Dependencies :
bash
Copy
1
pip install pandas numpy matplotlib seaborn statsmodels tensorflow sklearn
Open the Notebook :
Open Untitled4.ipynb in Google Colab or Jupyter Notebook.
Ensure all dataset files are present in the same directory as the notebook.
Run the Cells :
Execute the cells sequentially to perform data cleaning, analysis, and forecasting.
View Results :
The processed data (combined_data.csv) and visualizations will be generated during execution.
Analysis Highlights
1. Data Cleaning & Transformation
Unified multiple datasets by merging them on the Year column.
Converted large numbers into human-readable formats (e.g., B for billion, T for trillion).
Renamed columns for clarity (e.g., Oil exports (m³)).
2. Exploratory Data Analysis (EDA)
Visualized trends in oil prices, GDP, inflation, and other variables over time.
Compared oil exports and imports using bar charts.
Analyzed correlations between key variables using a heatmap.
3. Forecasting Models
ARIMA Model :
Used GDP as an exogenous variable to predict oil prices.
Generated forecasts up to the year 2070.
LSTM Neural Network :
Trained a nonlinear model to predict oil prices.
Adjusted predictions for future scenarios (e.g., net-zero pledges).
4. Scenario Analysis
Simulated two scenarios:
Current Trajectory : Includes geopolitical shocks and volatility.
Net-Zero Scenario : Assumes global efforts to reduce carbon emissions.
Forecasting Results
The project provides two sets of forecasts:

Raw Predictions : Unadjusted forecasts from the LSTM model.
Adjusted Predictions : Logistic decay applied to account for future constraints (e.g., reduced oil demand).
Key findings:

Oil prices are expected to fluctuate significantly due to geopolitical tensions.
The net-zero scenario predicts a gradual decline in oil prices as renewable energy adoption increases.
Contributions
Contributions to this project are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request.

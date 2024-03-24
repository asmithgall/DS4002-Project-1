# DS4002-Project-2-Gas-Price-Modelling

This is an attempt at predicting US Average Gas Prices based on a variety of monthly variables, including Unemployment, CPI, and economic indicators for Crude Oil, the S&P 500, and the XLE and VDE Energy ETFs. Using both Linear Regression and Gradient Boosting models, these variables are used to predict Gas Prices for the following month.

# Section 1
## Software and Platform Section
This project requires running scripts in both Python and R. Python scripts were run in Visual Studio Code, while R scripts were run in R Studio. In Python, we used the yfinance package in order to pull data from the Yahoo Finance API. We used the datetime package in order to do our date encodings and the Pandas package in order to do some preliminary data cleaning. Within R, we used lubridate for date handling and the xlsx package for preliminary data cleaning. The dplyr and ggplot packages were essential to add pipeline functionality and graphing ability in the scripts. Finally, the caret package was used for the actual modelling, having a variety of popular models available. The analysis was all carried out on the Mac OS platform.

# Section 2
## Documentation of the Project
Our repository contains three major folders. The first folder is the DATA folder. This folder contains the final_data.csv file which is ultimately fed into the modelling script. It also contains the PREPROCESSING subfolder, which contains the DOWNLOADS and API folders. The Downloads folder has four excel spreadsheets which were downloaded from online sources [2,3], listed in the data dictionary. It also contains the stuff.csv file which combines these all into a single csv. The API folder has the csv data pulled from the Yahoo Finance API [4]. All of this data is aggregated in the final_data.csv file but the file can be remade by running the 1 and 2 scripts. The second major folder is the SCRIPTS folder. This folder contains the scripts used to conduct analysis, from 1-3 in order of when to execute each script. Script 1 and 2 are preprocessing while Script 3 conducts the analysis. Finally, the OUPUT folder contains .jpg files of the graphs outputted from analysis.

# Section 3
## Instructions for Use
In order to reproduce this project, you will need R Studio, a Python script runner, and access to the Yahoo Finance API or text files from our repository. First, download the stuff.csv file from the DOWNLOADS subfolder inside DATA/PREPROCESSING. This data can also be alternatively downloaded by using the links in the data dictionary. Next, execute the first script, which will pull the Yahoo Finance API data using python. You will need to edit the script with your individual API key. This data can also be downloaded from the API folder within DATA/PREPROCESSING. Once you have the four csvs from the API and the stuff csv from downloads, execute script 2 in R studio which will combine them all into the final csv. After you have the data compiled, run the third script to carry out the analysis. This script creates both models using for testing and outputs the important graphs.

## References

[1] Factors Affecting Gasoline Prices - U.S. Energy Information Administration (EIA). https://www.eia.gov/energyexplained/gasoline/factors-affecting-gasoline-prices.php. Accessed 24 Mar. 2024.

[2] Federal Reserve Economic Data | FRED | St. Louis Fed. https://fred.stlouisfed.org/. Accessed 24 Mar. 2024.

[3] U.S. Regular All Formulations Retail Gasoline Prices (Dollars per Gallon). https://www.eia.gov/dnav/pet/hist/LeafHandler.ashx?n=pet&s=emm_epmr_pte_nus_dpg&f=m. Accessed 24 Mar. 2024.

[4] Yahoo Finance - Stock Market Live, Quotes, Business & Finance News. https://finance.yahoo.com/. Accessed 24 Mar. 2024.



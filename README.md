<<<<<<< HEAD
=======
# AIRCRAFT RISK ASSESSMENT FOR COMMERCIAL AND PRIVATE OPERATIONS


# Overview
This project is designed to  analyze the history of the Aviation data and decide which aircraft model has the lower risk for commercial and private enterprises.The analysis will help the company in determining which aircraft is safest to purchase and operate to minimize the potential risk of accidents.Dataset 'AviationData.csv will help in analysing by identifying the patterns,the trends and accidents rates based on the aircraft model,type of injuries, weather conditions and other factors that contribute to the risk of each aircraft.
# Business problem
Our company is expanding in Aviation industry and are interested in purchasing and operating airplanes for commercial and private enterprises,however they lack knowledge about the potential risks involved in an aircraft.They want to purchase an aircraft model which will not cause financial losses and also has low risk of accidents.
We will check on the history of the aviation data in different aircraft model and evaluate the accident count,severity of injuries and whether the aircrafts are for Private or Commercial purpose and generate Dataa driven insights to guide the company in decision making.
# The Data
The data was pulled from kaggle https://www.kaggle.com/datasets/khsamaha/aviation-accident-database-synopses which contain data from the National Transportation Safety Board that includes aviation accident data from 1962 to 2023 about civil aviation accidents and selected incidents in the United States and international waters.
# Questions to consider:
1. Which country had the highest number of accidents?
2. Which country had the highest cases of Fatal injuries?
3. Are there certain locations where accidents are most likely to occur?
4. In  which weather condition were those flights conducted?
5. In which weather conditions did most fatal accidents occur?
6. Which aircraft make had the highest Injury severity?
7. Which make and Model has lowest risk of injuries?
8. At which broad phase of fight did accident occur the most?
9. Which aircraft are we going to purchase for both private and commercial purposes with lowest risk of accidents?
10. What is the trend of accidents over the years?
# Data preparation and Cleaning
## objectives:
1. Loading files using python packages.
2. Inspecting the data and columns.
3. Handling missing and inaccurate data by identifying missing values and inaccurate values and fixing.
4. Ensure the desired observations are well organised.
# Import python libraries
# numpy for numerical computations  and mathematical calculations on arrays 
import numpy as np
# pandas for data manipulation and analysis and reading and writing csv files
import pandas as pd
# seaborn and matplotlib for data visualization
import seaborn as sns
import matplotlib.pyplot as plt
%matplotlib inline
# Loading the Data
>aviationData= pd.read_csv('AviationData.csv',encoding='ISO-8859-1',low_memory=False)
# previewing the dataset
#### Preview the first 5 rows of the data
>aviationData.head()
#### Preview the last 5 rows of the data
>aviationData.tail()
# Inspecting the data
##### Accesing information about the dataset
>aviationData.info(verbose=False)
##### Checking the number of rows and columns
>aviationData.shape
#### Checking the columns
>aviationData.columns
#### Calculating the summary statistics 
>aviationData.describe()
#### Calculating the summary statistics of categorical columns
>aviationData.describe(include='object')
#### Checking for column data types
>type(aviationData)
# Data Cleaning
#### creating a new copy of a Dataframe
>aviationData1 = aviationData.copy(deep=True
#### Cleaned data
>cleaned(aviationData)
>cleaned(aviationData1)
# Missing Values
#### Detecting missing values
>aviationData1.isna().sum().sum()
# Answering the data analysis questions by analysing through visualizations
# Visualizations
![image](https://github.com/user-attachments/assets/ab43581b-57b2-4ea9-b527-69777a8a011a)
![image](https://github.com/user-attachments/assets/0cc01eed-02f1-451b-895e-9b34d68c13ca)
![image](https://github.com/user-attachments/assets/697743d0-87be-4add-b3a2-62ec6504a1a4)
![image](https://github.com/user-attachments/assets/f20ecdd2-74c8-4765-afe0-a0a593be6768)
![image](https://github.com/user-attachments/assets/c617012a-54d0-4b1c-8503-25006a91c63b)
# Findings
1. private flights have slightly higher accident rates than the commercial flights but also have low injury severity rate.
2. Commercial flights experience few fatal injuries but depending on the model.
3. Based on the analysis,the aircraft model which posses low injury severity and accident rates are advised.
4. From my analysis,the weather condition did not affect much the performance of the aircraft .           
5. Most accidents happened during the VMC conditions which was a conditional suitable for flying so the weather did not influence the performance of the aircraft.
6. Apart from the data that is unknown,most accidents were caused when the airplane model was Landing.
7. I can advise  aircraft model like Naval Aircraft Factory N3N for private purposes as it has low injury severity and accidents
8. For commercial purpose,I can advise Public Aircraft vickers VC10  as it has low accident and fatality rate with a number of uninjured.
# Metrics of success
My project would be successful if I would be able to identify:
1. Aircrafts models with high percentage of minor injuries or no injuries and low percentage of fatal injuries are preffered.
2. Aircraft models with lower  accident rates are preferred and also identify aircrafts with high accident rates and serious fatal injuries so as to avoid them.
3. Aircraft models with low cost effectiveness but has low accidents and injury rates for investment.
# Recommendations
1. Identify aircraft models with high risk of accident with fatal and serious injuries as they would posses a high risk and avoid them.
2. Prioritize aircraft model with low risk of Fatal and Injury rates.
3. Regular update  risk assessment and re-evaluate aircraft models as new data is updated.
# Conclusion
There is differences between safety performance of both Private and Commercial aircraft.
Low risk Aircraft model with low accident rate and low injury severity has been identified
Ensure a balance between safety and operational efficiency.














>>>>>>> 8791221802d4678f7d71ac28c99b9e655e8a41d6

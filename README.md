# Predicting Number of Insurance Benefits

<p align="center">
  <img src="https://github.com/kellyshreeve/predicting-insurance-benefits/blob/main/images/insurance_clipart.png"
  width="400"
  height="300"
  alt="Insurance clip art">
</p>

# Project Overview

An imbalanced classification machine learning project predicting two outomes: 1) whether a customer will use insurance benefits, and 2) how many benefits a customer will use. Pipelines, GridSearchCV, and class balancing techniques are used to fit and tune kNN binary classification, logistic regression, kNN multi-class classification, and random forest multi-class classification. Class balancing techniques of SMOTE, SMOTENN, and class weighting are applied.

# Installation and Setup

## Codes and Resources Used

  - <b>Editor Used</b>: Visual Studio Code
  - <b>Python Version</b>: 3.10.9

## Python Packages Used

  - <b>General Purpose</b>: ```numpy```  
  - <b>Data Manipulation</b>: ```pandas```  
  - <b>Data Visualization</b>: ```matplotlib, seaborn```  
  - <b>Machine Learning</b>: ```imblearn, sklearn```  

## Installing development requirements

```pip install -r requirements.txt```

# Data

## Source Data

sql_result_01.csv
  * *company_name*: taxi company name
  * *trips_amount*: the number of rides for each taxi company on November 15-16, 2017  

sql_result_04.csv
  * *dropoff_location_name*: Chicago neighborhoods where rides ended
  * *average_trips*: the average number of rides that ended in each neighborhood in November 2017  

sql_result_07.csv
  * *start_ts*: picup date and time
  * *weather_conditions*: weather conditions at the moment the ride started
  * *duration_seconds*: ride duration in seconds

## Data Acquisition

The data were retrieved through HTML parsing and SQL queries of a large database provided by TripleTen. 

## Data Preprocessing

Data were checked for missing values and duplicates. None were found and no imputation was necessary.
 
# Code Structure
```
  ├── LICENSE
  ├── README.md          
  │
  ├── images
  │   └── car-picture.png    
  │
  ├── notebooks  
  │   └── Zuber_Analysis.ipynb 
  │
  └── requirements.txt  
```

# Results and Evaluation

<p align="center">
  <img src="https://github.com/kellyshreeve/Zuber_Rides_Analysis/blob/main/images/trips-company.png" 
  alt="Bar graph of total trips by company">
</p>

<p align="center">
  <img src="https://github.com/kellyshreeve/Zuber_Rides_Analysis/blob/main/images/drop-offs.png" 
  alt="Bar graph of average drop offs by neighborhood">
</p>

<p align="center">
  <img src="https://github.com/kellyshreeve/Zuber_Rides_Analysis/blob/main/images/hypothesis-test.png" 
  alt="Statistical output of two-indpendent samples t-test comparing average trip length in good vs bad weather">
</p>

# Future Work

# Acknowledgments/References


# Predicting Number of Insurance Benefits

<p align="center">
  <img src="https://github.com/kellyshreeve/predicting-insurance-benefits/blob/main/images/insurance_clipart.png"
  width="400"
  height="300"
  alt="Insurance clip art">
</p>

# Project Overview

An imbalanced classification machine learning project predicting two outomes: 1) whether a customer will use insurance benefits, and 2) how many benefits a customer will use. Pipelines, GridSearchCV, and class balancing techniques are used to fit and tune kNN binary classification, logistic regression, kNN multi-class classification, and random forest multi-class classification. Class balancing techniques of SMOTE, SMOTEENN, and class weighting are applied.

# Installation and Setup

## Codes and Resources Used

  - <b>Editor Used</b>: Visual Studio Code
  - <b>Python Version</b>: 3.10.9

## Python Packages Used

  - <b>General Purpose</b>: ```numpy```  
  - <b>Data Manipulation</b>: ```pandas```  
  - <b>Data Visualization</b>: ```matplotlib, seaborn```  
  - <b>Machine Learning</b>: ```imblearn, sklearn```  

# Data

## Source Data

insurance_us.csv
  * *gender*: customer's gender  
  * *age*: customer's age    
  * *salarye*: customer's yearly income  
  * *family_members*: number of additional members in the family  
  * *insurance_benefits*: number of benefits used  
 
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


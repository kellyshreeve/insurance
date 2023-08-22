# Predicting Insurance Benefits

<p align="center">
  <img src="https://github.com/kellyshreeve/predicting-insurance-benefits/blob/main/images/insurance_clipart.png"
  width="400"
  height="300"
  alt="Insurance clip art">
</p>

# Project Overview

An imbalanced classification machine learning project predicting two outomes: 1) whether a customer will use insurance benefits, and 2) how many benefits a customer will use. Pipelines, GridSearchCV, and class balancing techniques are used to fit and tune kNN binary classification, logistic regression, kNN multi-class classification, and random forest multi-class classification to maximize F1 score (binary) and macro-averaged F1 score (multi). Class balancing techniques of SMOTE, SMOTEENN, and class weighting are applied.

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

<b>Features</b>
  * *gender*: customer's gender  
  * *age*: customer's age    
  * *salarye*: customer's yearly income  
  * *family_members*: number of additional members in the family  

<b>Targets</b>
  * *insurance_benefits*: number of benefits used  
  * *received_benefits*: whether customer received benefits or not
 
## Data Acquisition

The data were provided by TripleTen's Data Science bootcamp. The full dataset is loaded into the notebook but is proprietary information and cannot be shared online.

## Data Preprocessing

Data were checked for missing values and duplicates. None were found and no imputation was necessary.
 
# Code Structure
```
  ├── LICENSE
  ├── README.md          
  │
  ├── images
  │   └── insurance_clipart.png    
  │
  └── notebooks  
      └── insurance_analysis.ipynb  
```

# Results and Evaluation

<p align="left">
  <img src="/images/eda.png"
  width="500"
  height="500"
  alt="sns pair plot of variables colored by receiving benefits">
</p>

<p align="left">
  <img src="/images/binary_results.png" 
  width="500"
  height="250"
  alt="Results of binary classification model tuning">
</p>

<p align="left">
  <img src="/images/binary_test.png"
  width="400"
  height="100"
  alt="Test results of logistic regression with threshold = 0.43">
</p>

<p align="left">
  <img src="/images/multi_results.png"
  width="600"
  height="250"
  alt="Results of multi class classification model tuning">
</p>

<p align="left">
  <img src="/images/multi_test.png"
  width="550"
  height="100"
  alt="Test results of random forest multi class classification">
</p>




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
  * *salary*: customer's yearly income  
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

Pairplot of datset, colored by received insurance benefit:  
<p align="left">
  <img src="/images/eda.png"
  width="550"
  height="550"
  alt="sns pair plot of variables colored by receiving benefits">
</p>

There is clear clustering in whether someone receives benefits by age.

<p align="left">
  <img src="/images/binary_results.png" 
  width="500"
  height="250"
  alt="Results of binary classification model tuning">
</p>

Logistic regression with threshold optimized to 0.43 achieved an average F1, ROC AUC, accuracy, precision, and recall of 1.0 on the cross-validated training data.

<p align="left">
  <img src="/images/binary_test.png"
  width="310"
  height="90"
  alt="Test results of logistic regression with threshold = 0.43">
</p>

The logistic regression with threshold = 0.43 again achieved scores of 1.0 across all scores.

<p align="left">
  <img src="/images/multi_results.png"
  width="690"
  height="250"
  alt="Results of multi class classification model tuning">
</p>

The random forest model with SMOTEENN balanced and weighted classes achieved the best multi-class classification results, scoring a macro-averaged F1 score of 0.9894.

<p align="left">
  <img src="/images/multi_test.png"
  width="510"
  height="100"
  alt="Test results of random forest multi class classification">
</p>

The random forest model with SMOTEENN and class weighting achieved similar results on the test set, achieving an F1 macro of 0.9764.

# Conclusions


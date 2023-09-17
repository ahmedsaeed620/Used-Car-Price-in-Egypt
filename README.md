# Used-Car-Price-in-Egypt
  - [Demo](#demo)
  - [Overview](#overview)
    - [Dataset Descrption](#dataset-descrption)
  - [EDA](#EDA)
  - [Best Model selection](#best-model-selection)
    - [Best parametes](#best-parametes)
    - [Feature importances](#feature-importances)
  - [Technologies Used](#technologies-used)


## Demo

## Overview
This project aims to predict typical bus costs in Egypt, so that buyers can make an informed purchasing decision using data collected from colorful sources spread across colorful areas in Egypt. We realize that buses are not just a means of transportation, but an expression of our own tastes and needs. The choice may be limited depending on our budget, however, we can take advantage of regular car demand to enjoy the luxury brands we love at lower prices. By examining the available data, we will provide information about the cost of manned buses based on the brand, model, condition and other dependent factors. This will enable buyers to make an informed purchasing decision and choose a vehicle that suits their requirements and budget.

### Dataset Descrption

Dataset used here is from a [Kaggle Dataset ](https://www.kaggle.com/datasets/abdo977/used-car-price-in-egypt). 

* Size of Dataset set: 14741 records
  
* **Features**: 
    - Brand: The brand of the car
    - Model:	The Model of the car
    - Body: The Body of the car
    - Year: The year or edition of the model
    - Color: The color the car
    - Fuel: The type of fuel used by the car
    - Kilometers: The range kilometers driven in the car by the previous owner(s) in KM
    - Engine: The displacement volume of the engine in cc
    - Transmission: The type of transmission used by the car
    - Price: The price of the used car
    - Gov: The Gov in which the car is being sold or is available for purchase
## EDA

In this section of the project, the data is explored to see the patterns and trends and observe interesting insights. Below are some interesting observations generated.

-  ```Kilometers_Driven``` and ```Engine``` are Handling The range of value.
-  ```Age_of_Car``` Create a new column using the ```Year``` column.
-  ```Price``` Multiply the price by 1000
- ```Brand```,```Model```,```Body```,```Color``` ```Fuel```, ```Transmission``` and ```Gov``` are encoded using **bainary encoding** as they have lot of categories.
- 
## Best Model selection

The data is trained on Linear Regression, Ridge, PolynomialFeatures , Decision Tree Regressor, Random Forest Regressor, VotingRegressor, BaggingRegressor, AdaBoost Regressor, GradientBoostingRegressor, and XGBoost. GradientBoostingRegressor turned out to be the best model with accuracy= 88.10.


### Best parametes

``` python
{'Model_fit__n_estimators': 300,
  'Model_fit__max_depth': 5 }
```

### Feature importances

<img src = "https://github.com/ahmedsaeed620/Used-Car-Price-in-Egypt/blob/main/Images/Feature_Importances.png" width = 850 height = 400/>

## Technologies Used

[![](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=darkgreen)](https://www.python.org)
[![](https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/stable/)
[![](https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org) 
[![](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![](https://img.shields.io/badge/Plotly-239120?style=for-the-badge&logo=plotly&logoColor=white)](https://plotly.com) 
[![](https://img.shields.io/badge/conda-342B029.svg?&style=for-the-badge&logo=anaconda&logoColor=white)](https://www.anaconda.com)


Link My accaount in Kaggle : [Ahmed elsaied](https://www.kaggle.com/ahmedsaied3122)

Link My notebook in Kaggle : [Used Car Price in Egypt](https://www.kaggle.com/code/ahmedsaied3122/used-car-price-in-egypt)


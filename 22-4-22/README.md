
# Problem Statement

ABC is a car rental company based out of Bangalore. It rents cars for both in and out stations at affordable prices. The users can rent different types of cars like Sedans, Hatchbacks, SUVs and MUVs, Minivans and so on.

In recent times, the demand for cars is on the rise. As a result, the company would like to tackle the problem of supply and demand. The ultimate goal of the company is to strike the balance between the supply and demand inorder to meet the user expectations.

The company has collected the details of each rental. Based on the past data, the company would like to forecast the demand of car rentals on an hourly basis.

![Logo](https://cdn1.vectorstock.com/i/1000x1000/86/00/logo-for-car-rental-and-sales-vector-25468600.jpg)


## Aim Of Project :-

- forecast the demand of car rentals



## Approach to solve problem 
Step 1: Importing the Relevant Libraries

Step 2: Data Inspection

Step 3: Data Cleaning

Step 4: Exploratory Data Analysis

Step 5: Building Model


![Logo](https://www.favouriteblog.com/wp-content/uploads/2017/07/Machine-Learning-Process.png)



## Install dependecies
numpy 
```
pip install numpy
```
pandas
```
pip install pandas
```
matplotlib
```
pip install matplotlib
```

## Features of dataset:

| Features |
| :-------- |
| `Date` |
| `Hour` |
| `Demand` |

## Approaches:-
1. Apply multiple ML algorithms get there RMSE value and Select 2 of them and perform Hyperparameter Tuning.
2. Use concepts of Deep Learning.
3. Use Voting Classifier and use multiple ml algos same time.

## Steps -
i) import  numpy,  pandas, matplotlib, datetime, calendar  & sklearn.

ii) Read both the train and prediction csv.

iii) Check details about data by describe function.

iv) Check if there is any NAN values.

v) Create a separate column fro date, month & year from Datw dd-mm-yy column. 
  - Try to extract season but not succeed.
  
vi) Visualize data by diffrent graphs

vii) Split dataset in train & test

viii) Tried multiple ml algos and calculate rmse value.

ix) Select 2 of all ml algos and perform Hyperparameter Tuning by GridSearch.

x) Apply Standard Scaler and use Deep Neural Network.

xi) Use Voting Classifier(knn, XGB, Random Forest) and use multiple ml algos same time.



## Result

|    |**Model** | **RMSE train**    | **RMSE test %**             |
| :- | :-------- | :------- | :------------------------- |
| 1| `Random Forest` | 12.7492 |  	33.7474 |
| 2|`SVR` | 38.3123 |  36.9523 |
| 3|`XGB` | 35.1130 |  	34.250 |
| 4 |`DNN` |  	41.03 | 41.68|
| 5 |`Voting Classifier` |  	32.56 | 34.00|






Analytics Vidhya -JOB-A-THON-NOV-2022

RANK: 92/6388

SCORE: 465.66

Problem Statement : In this, there is a research organistaion who has energy consumption data of world from 2008 to 2018. And to meet future requirement he want to forecast energy demand of world. So they can know that how much resourcesthey need to meet that requirment.

In our dataset we have two columns : i) date & hours ii)energy demand

So we will try it by two ways: first by normal Regression method, LSTM and than Facebook FBProphet.

Steps:
1. We will install required libraries: pystan=2.19, fbprophet.
2. Import libraries: numpy, pandas, matplotlib, sklearn.
3. Read train and test csv.
4. Evaluate dataset by describe and info functions.
5. Handle nan values either by filling mean value, ffill method or will drop it.
6. Extract date, year, month, day etc. from date & hour column.
7. Split the data: train and test.
8. First use normal regression algorithm: Linear & SVR.
9. Than use fbprophet
  i)Convert as (ds, y) format.
  ii)Calling model and perfrming fit operation.
    As energy demand is effected by months, just like in summer or particular month demand of energy hiked.
    Also adding country holidays, because that time energy demand increases.
    
So mean absolute error by LR and SVR are 266 and 260.
So mean absolute error by fbprophet is 134.


Things are in testing :
1. Hyper parameter tuning fbprophet model.
2. Use LSTM generate result.
3. And than use average of fbprophet and LSTM.

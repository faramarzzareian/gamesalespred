# Video Game Sales Prediction - ML Project
The Project is Coded for Machine learning Course and it is studied by (Prof.Lorenzo Rosasco, Prof.Alessandro Verri) in Univerity of Genova,italy 2018/2019

This project is predicting the video games sales in several different Area and it is coded in python.

project is a supervised-Regression.

#  Data Set 

After search in kaggle I found several game related data sets but i choosed to take the video games sales for predicting the sales . 
first of all I had to pre-process the data set I choosed then use the algorithms : SVM (support vector machines) , Linear Regression 
and in the final we have accuracy and cross validation values.
.csv format file and it contains 16500 rows and 11 column, the number for each sales are defined as million dollar.

JP = JAPAN SALES

EU = EUROPEAN SALES

NA = NORTH AMERICA SALES

GLOBAL SALES = SALES AROUND THE WORLD

PUBLISHER = THE COMPANY MADE A GAMES

SALES = IN MILLION DOLLAR

PLATFORM = Release platform for the game

YEAR = Year of release (Since 1980 to 2016)


# Steps of Project 
1- Data Pre-Processing

2- Implementing the Algorithms

3- Results

# Data Pre-Processing
Data set Link : https://www.kaggle.com/gregorut/videogamesales
with 16579 records for each column and 11 column.

1-First step is loading the data set in program you want to write the codes , for me it is a jupiter note book of anaconda ( www.anaconda.com)

2-the second part I start to find how many null we have so with the code we find how many of our datas in which column are null and then after we found that out 
which type of data is null we can do the right action for example in this dataset I have nulls in my "Year" column and we have two option to 
set a mean of all other years into null and the other option is if our null data is not that much in compare of our rows  we can delete entire the rows with null data but this is not a good option and 
it will change the results dramatically

3-so, in the next part I drop the columns which i dont want to use with
and the main purpose of drop for me is because my laptop is so old and process will take more times.
beside of drop some column I add some code to drop some of data from buttom because of the old laptop , so can delet that part.

4-its time for choosing Features X and Labels Y
I choose the name of games as X and the mount of their sales as Y.

5- in this part I splite the data set into Training and Test sets.

# Implementing the Algorithms

1-Linear Regression

2-SVR ( SUPPORT VECTOR MACHINES )
3- knn ( RMSE ) I used this code exprimentaly to see how knn regression works and in this code I used k=1 to 100 and the result is Root Mean Square Error , so when our error is lowest possible it means its better. and in this case k=7 is the best possible

# Results

Linear regression : 

                    cross-validation 68%

                    accuracy 73%
                    
SVR               : 

                    cross-validation 57%

                    accuracy 58%           
                    
KNN ( RMSE ) 


RMSE value for k=  1 is: 0.5596475260681059


RMSE value for k=  2 is: 0.47944528353956


RMSE value for k=  3 is: 0.4754904773280576


RMSE value for k=  4 is: 0.4703379710903737


RMSE value for k=  5 is: 0.47438705444336976


RMSE value for k=  6 is: 0.4740020658967919


# RMSE value for k=  7 is: 0.4623625231010482


RMSE value for k=  8 is: 0.46392061552023933


RMSE value for k=  9 is: 0.4674917209011803


RMSE value for k=  10 is: 0.46918482364345615


RMSE value for k=  11 is: 0.4719602390941327


RMSE value for k=  12 is: 0.47209735714686746
               

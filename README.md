# SQL-Injection-Detection Using Machine Learning

## What is SQL Injection(SQLi)?
SQL injection is a code injection technique in which malicious SQL statements are inserted into an entry field for execution. It generally allows an attacker to view data that they are not normally able to retrieve. It is one of the most common web hacking techniques.

![image](https://user-images.githubusercontent.com/96000840/217074588-ee12b1a6-8eb2-44cd-a832-a4ce15fd2dd7.png)

## How SQLi queries are created? How they are used to get information and types of SQLI queries with a simple example.
* Consider : You open a website & it asks for login credentials to login i.e. "userid and password".
* Consider the userid = xyz and password = 123
* The web application internally creates a sql query to validate the userid and password i.e sql query will be: Select * from users where userid = xyz and password = 123.

## Data Collection
The set of normal and injected queries are collected from open source service named as Kaggle. In this dataset 10000 random normal(legitimate) queries, about 5000 Injected queries and 800 Plain queries are collected to train the ML models.

## Machine Learning
It is a Supervised Machine Learning(classification) task. Algorithms considered to train the dataset in this project are:
* Decision Tree
* Random Forest
* Adaboost
* XGBoost
* Gradient Boosting Machine
* Light Gradient Boosting Machine
* Autoencoder Neural Network
* Support Vector Machines

## Refrences
* [Detection of SQL Injection Attack Using Machine](https://www.mdpi.com/2624-800X/2/4/39/pdf)
* [Ensemble Machine Learning Approaches for Detection of SQL Injection Attack --By Umar Farooq](https://hrcak.srce.hr/file/367636)

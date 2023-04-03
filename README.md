# SQL-Injection-Detection Using Machine Learning

## What is SQL Injection(SQLi)?
SQL injection is a code injection technique in which malicious SQL statements are inserted into an entry field for execution. It generally allows an attacker to view data that they are not normally able to retrieve. It is one of the most common web hacking techniques.

![image](https://user-images.githubusercontent.com/96000840/217074588-ee12b1a6-8eb2-44cd-a832-a4ce15fd2dd7.png)

## How SQLi queries are created? How they are used to get information and types of SQLI queries with a simple example.
* Consider : You open a website & it asks for login credentials to login i.e. "userid and password".
* Consider the userid = xyz and password = 123
* The web application internally creates a sql query to validate the userid and password like : **Select * from users where userid = xyz and password = 123**.
* The attacker/hacker who does not has login credentials, he/she will Input the credentials like : **Userid = or 1=1 -- Password = 123**
* Internally web application creates a sql query like : **Select * from user where userid = or 1=1 -- and password = 123**
* Userid contains or keyword. Or gate always returns true when one of the input is true. i.e 1=1 is always true. And -- comments out rest of the query.
* The result will be true. And attacker can get access to all userid and password in database.
* This is the basic understanding of How SQLi queries are used to get access to the database. For more information visit : [SQL Injection](https://www.w3schools.com/sql/sql_injection.asp)

## Data Collection
The set of normal and injected queries are collected from open source service named as Kaggle. This dataset contains two columns: Query, label. Label column contains 1 and 0 values. Where 1 represents that Particular Query that can get access to database i.e SQLI query and 0 represents that can not get access to database i.e it can be Normal Sql query or plain text.

## Machine Learning
It is a Supervised Machine Learning(classification) task. 

## Refrences
* [Detection of SQL Injection Attack Using Machine](https://www.mdpi.com/2624-800X/2/4/39/pdf)
* [Ensemble Machine Learning Approaches for Detection of SQL Injection Attack --By Umar Farooq](https://hrcak.srce.hr/file/367636)

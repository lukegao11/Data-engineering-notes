# Data engineering notes
a notebookish diary for a data engineer wannabe




## 8/6/2022

**Data pipeline design patterns**

source: https://youtu.be/v67JHa4MrnQ

1. Extract transform and load (ETL)


***What is sink in data pipeline?***

A *sink*, on the other hand, is a consumer of data, providing logic for the transformation and publication of data emitted from related sources. In effect, a sink describes a chain of handlers. The chain starts with zero or more transformers and ends with one or more publishers.

2. Extract load and transform (ELT)


## 8/10/2022

SQL learning

A. 

  DENSE_RANK() VS RANK()

  ORDER BY (REQUIRED)

  PARTITION BY (OPTIONAL)
  
  
  <img width="675" alt="Screen Shot 2022-08-10 at 14 09 52" src="https://user-images.githubusercontent.com/99423162/183985737-c161c503-6820-402d-952a-489f844f69b4.png">

B.

  Union is faster than (condition) and (condition)


## 8/16/2022
***SUM() AND COUNT() IN mySQL***

source (https://stackoverflow.com/questions/39670039/mysql-what-is-the-difference-between-sum-and-count)

SELECT SUM(USER_NAME =  'JoeBlow') 

SELECT COUNT(USER_NAME =  'JoeBlow') 

The first query returns the number of times the condition is true, because true is 1 and false is 0.

The second query returns the complete record count because count() does not care about the content inside it, as long as the content is NOT NULL. Because count(1) and count(0) are still values and both get counted.

To get the correct return value for the second query you would have to make the result of the condition be null (instead of 0) to not being counted.




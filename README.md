# titanic_analysis for Excel
The purpose of analysis is to find the total number of survivors and non surivivors
The average age of survivors and non survivors
Creating visulaiztion the distribution of survivors
Summary
Cleaned the data by using filters to represent empty cells by yellow color
Calculated average age of survivors and non survivors
Calculated number of survivors by PClass
Created bar charts and pie charts to view the distribution of survivors



Assume you have imported the dataset into a SQL database. Write SQL queries to answer the following questions:
1 )What is the total number of passengers?
SELECT *
 FROM new_schema.titanic;
 SELECT COUNT(*)
 AS total_passengers
 FROM titanic
 
2)What percentage of passengers survived?
SELECT*
FROM new_schema.titanic;
SELECT 
    (SUM(Survived) * 100.0 / COUNT(*)) 
FROM  titanic



3)How many passengers were in each class (Pclass)?

SELECT *
 FROM new_schema.titanic;
 SELECT Pclass,
 COUNT(*) AS COUNT
 FROM titanic
 GROUP BY Pclass


4) What was the average fare for survivors and non-survivors?



SELECT
    survived, AVG(fare) AS average_fare
FROM titanic
GROUP BY survived;

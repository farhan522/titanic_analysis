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
What is the total number of passengers?
SELECT *
 FROM new_schema.titanic;
 SELECT COUNT(*)
 AS total_passengers
 FROM titanic
 
What percentage of passengers survived?
How many passengers were in each class (Pclass)?

SELECT *
 FROM new_schema.titanic;
 SELECT Pclass,
 COUNT(*) AS COUNT
 FROM titanic
 GROUP BY Pclass


What was the average fare for survivors and non-survivors?

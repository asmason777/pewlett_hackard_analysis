# Pewlett-Hackard Analysis
---
## Overview of Project

### Purpose

Pewlett-Hackard is a large company that employs approximately 300,000 people. To ensure stability it is important to be able to estimate the number of employees eligible to retire over the next several years to determine hiring decisions going forward. There is an expected large number of soon-to-be retirees known as the “silver tsunami.” Using the database SQL, it is possible to combine data pulled from multiple sources (tables) to make new tables that output the information together making it simpler to analyze.

## Tables

### Methodology

The raw data was initially pulled into six different spreadsheets – each including different employee and department information. SQL can combine columns from two different databases if each database has a column that contains identical information. The information must also be unique meaning that it cannot be repeated a second time in the column. Throughout the different spreadsheets, two columns met that criteria: employee number and department number. After the columns from the different spreadsheet are combined into a new table, the data can then be sorted by employee birth date to pull a list of employees that are at or near retirement age. Finally, the list can then be scrubbed to reduce any duplicate employee names as employees that have had more than one job title during their time at the company may appear more than once.

A second table was also created to identify experienced employees that might be able to act as mentors to younger and/or new hires. This table was created using the same logic as the prior table with the only exception being that the employees chosen for this list were younger and thus assumedly experienced but further from retirement. 

### Table Observations
 
* Roughly 90,000 of 300,000 total employees (approximately 30 percent of all Pewlett-Hackard employees) are at or near retirement age.  
  
* Over 73,000 of the 90,000 are classified as Engineers or Senior Engineers.  
 
* Senior Engineers make up almost 30,000 of the 90,000 employees on the “retirement list.”  

* The list for mentors to help train employees for the expected job vacancies is less than 2,000 employees and of those only 213 are Senior Engineers.   

[![Retirement-list.png](https://i.postimg.cc/vBDXkrLV/Retirement-list.png)](https://postimg.cc/N9q1rrns)          [![Mentors-pivot.png](https://i.postimg.cc/5yCgNfr9/Mentors-pivot.png)](https://postimg.cc/kR7KTP9L)  

### Summary

The observations from the two tables above prove that the expected “silver tsunami” is indeed an issue that needs to be addressed immediately. Not only are one-third of all employees expected to retire within several years but currently there are only 213 Senior Engineers on staff available to mentor upwards of 30,000 vacancies. Based on these findings, the following recommendations are offered:

1.	Run a query that can return the average age by job title for past employees that left the company when they were 64 or older. This would likely provide insight as to the average age an employee retires. With the trend that many employees now work well past age 65, it would be helpful to confirm if this trend exists within the company so that the timeframe for training new and/or less experienced employees could be extended.

2.	Run a second query to find mentors not based on age but rather total time employed with Pewlett-Hackard. While older employees are more likely to be the most experienced, employees that have extensive time working for the company likely could also be excellent mentors. Thus, employees with 10 years or more at the company should be considered.

3.	Based upon the results of the two queries, design a mentoring program that allows time for replacements to be hired and trained. The mentors from this program would include those near retirement age as well as any employee that has been with the company ten years or more.

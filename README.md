# Pewlett-Hackard-Analysis

Build Employee Database with PostgreSQL and perform SQL queries to explore and analysis data.

## Overview of the analysis

The purpose of this analysis is to create two tables:
- The first one to determine the number of retiring employees and their position titles.
- And the seconde one to identify employees who are eligible to participate in a mentorship program. 
- Then prepare a report that summarizes the analysis that will help Boby's manager for the "silver tsunami" wave as many current employee reach retirement age.

Within the first table, we included information such as employee number, first and last name, position title, and start and end date. 

In the second, we added employee number, first and last name, birth date, start and end date, and position title.

## Resources

- Software : PostgresSQL Version 12
- All the Data : [Pewlett-Hackard-Analysis](/Pewlett-Hackard-Analysis/Data)


## Storage of the Data

Pewlett Hackard currently stores their employee data in 6 different csv files. Here is the entity relationship diagram of those datasets.

![EmployeeDB](/EmployeeDB.png)

## Results 
### Deliverable 1

Three tables was created in this deliverable.

1- The first table holds all the titles of current employees who were born between January 1, 1952 and December 31, 1955.

[Retirement_titles](/Data/retirement_titles.csv)

![Retirement_titles](/Data/retirement_titles.PNG)

2- The second table we removed duplicates titles that the employee may have switched over the years and kept only the most recent title of each employee.

[unique_titles](/Data/unique_titles.csv)

![unique_titles](/Data/unique_titles.PNG)

3- The third one retrieved the number of employees by their most recent job title who are about to retire.

[retiring_titles](/Data/retiring_titles.csv)

![retiring_titles](/Data/retiring_titles.PNG)

***Analysis of Deliverable 1***

- Almost a third of the retirees are Senior Engineers, while the other third includes the rest of the Senior Staff.
- Only 2 Managers are retiring.
- The rest of the count is dispatched between Engineer, Staff, Technique Leader and Assistant Engineer.
- As a result, The hiring priority of Pewlett-Hackard should be focused on replacing the Senior Engineer and Senior Staff positions.

### Deliverable 2

In this deliverable we created only one table that holds the employee eligible for mentorship program.

[mentorship_eligibilty](/Data/mentorship_eligibilty.csv)

![mentorship_eligiblity](/Data/mentorship_eligiblity.PNG)


***Analysis of Deliverable 2***

From the results above, 

# Pewlett-Hackard-Analysis

Build Employee Database with PostgreSQL and perform SQL queries to explore and analysis data.

## Overview of the analysis

The purpose of this analysis is to create two tables:
- The first one to determine the number of retiring employees and their position titles.
- And the second one to identify employees who are eligible to participate in a mentorship program. 
- Then prepare a report that summarizes the analysis that will help Boby's manager for the "silver tsunami" wave as many current employee reach retirement age.

Within the first table, we included information such as employee number, first and last name, position title, and start and end date. In the second, we added employee number, first and last name, birth date, start and end date, and position title.

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

- There are 90 398 employee who are likely to retire soon.
- Almost a third of the retirees are Senior Engineers 29 414, while the other third includes the rest of the Senior Staff 28 254.
- Only 2 Managers are retiring and need to be replaced.
- The rest of the count is dispatched between Engineer 14 222, Staff 12 243, Technique Leader 4502 and Assistant Engineer 1761.
- As a result, The hiring priority of Pewlett-Hackard should be focused on replacing the Senior Engineer and Senior Staff positions.

### Deliverable 2

In this deliverable we created only one table that holds the employee eligible for mentorship program by filtering on the employees born in 1965 and have current roles with no termination dates. 

[mentorship_eligibilty](/Data/mentorship_eligibilty.csv)

![mentorship_eligiblity](/Data/mentorship_eligiblity.PNG)


***Analysis of Deliverable 2***

The breakdown for this analysis is:

- There are 1550 employee eligible for the mentorship program dispatched as the following:
  - 63 Assistant Engineer 
  - 400 engineer
  - 285 Senior engineer
  - 430 Senior staff
  - 294 Staff
  - 77 Technique leader
  - There is no manager eligible for this program!

## Summary

By comparing the results of the two deliverables, we can see that there is a 90398 potential positions that need to be filled due to the retirement wave, where there is only 1550 employee currently eligible to mentor the new hired employees. This actively demonstrate that there is one mentor for every 58 new hired employee. 

Using the same logic for the rest of the titles we came up with the following findings:
- One for 103 new senior engineer
- One for 65 new senior staff
- One for 35 new Engineer
- One for 41 new staff 
- One for 58 new technique leader 
- One for 27 new assistant engineer

Giving those results, we can say that it's a very big amount of work for the existing employee in order to mentor the the new employee joigning the company.

As a results, If we change to criteria for the mentorship program to employees born between 1962 and 1965 those numbers drop to one mentor for every 1 to 2 new hired employee approximatly.
By changing the pool of eligible employees, this program has a strong chance to succeed and to give better results. More employees will be incentivized to mentor if they are only mentoring 1 to 2 people instead of having 50+ people. New employee will obtain more information from a one to one metoring compared to a group mentoring that would likely happen in the first situation.



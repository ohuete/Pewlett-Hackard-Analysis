# Pewlett-Hackard-Analysis
## Overview
### Purpose and Background
The purpose of this project is to create Entity Relationship Deiagrams (ERD's) and design tables using Structured Query Language (SQL). Pewlett Hackard is a well established company employing thousands of people. As they rapidly begin to lose employees to retirement, they are looking for ways to fill positions and distribute retirement packages for those who qualify. Applying data modeling, engineering, and analysis, I have helped Pewlett Hackard build a brand new and upgraded version of their employee data base with SQL. After I created various ERD's for Pewlett Hackard, they needed to further narrow their data. More specifically, to determine the number of retiring employees per job title and to identify employees who are eligible for their new mentorship program. 
### Resources 
- Postgres
- pgAdmin
- SQL
## Results
 - First, I joined the "titles" table with the "employees" tables to create one table holds all relevant employee information such as: Employee Number, First and Last Name, Job Title, From and To Date. Below is an image of the "retirement_titles" table. 

<img width="674" alt="Screen Shot 2022-08-05 at 1 52 13 PM" src="https://user-images.githubusercontent.com/107595127/183160828-84e9fe61-1dfa-41e0-b66f-1fb3be6d0307.png">

- As you can see, some employees appear more than once with different job titles. This is not quite what we want. I narrowed the results to create a table wit only the most recent title for each employee. Below is an image showing only the first ten results of the new table called "unique_titles".

<img width="523" alt="Screen Shot 2022-08-05 at 1 53 30 PM" src="https://user-images.githubusercontent.com/107595127/183160967-1af8da5e-be82-4408-90de-8b74f9377aeb.png">

- Still, the table is too large. It countains an exhaustive list of each employee that is retiring. To make it easier to read, I added a new table that only shows the number of employees retiring from each job title. Below is an image of the new consise "retiring_titles" table. 

<img width="214" alt="Screen Shot 2022-08-05 at 1 55 28 PM" src="https://user-images.githubusercontent.com/107595127/183161785-031e2144-9bfb-4a6d-b8ee-09729f2c8237.png">

- Now that we know who is retiring, the number of employees and their job titles, we can determine who is eligible for the mentorship program based on birth date. The new table contains employee number, first and last name, birth date, from and to date, and job title. Take a look at what the new "mentorship_eligibilty" table below. 

<img width="724" alt="Screen Shot 2022-08-05 at 2 57 43 PM" src="https://user-images.githubusercontent.com/107595127/183216743-6215c059-e51c-44e1-bcbb-55bcc974c870.png">

## Summary
Pewlett Hackard is looking at over 74,000 employees eligible for retirement. Based on the tables provided, there are more than enough current employees available for the mentorship program. The managers job title only has two retiring so they are either fine in that department or must keep them as mentors. Since every other department has at least 1,000 employees retiring, Pewlett Hackard probably cannot keep everyone as a mentor. A table to determine who exactly Pewlett Hackard would like to initiate into their mentorship program and who receives the reitrement package. 

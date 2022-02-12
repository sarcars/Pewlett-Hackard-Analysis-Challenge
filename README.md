# Pewlett-Hackard-Analysis-Challenge
Module 7 challenge (SQL)


## Overview of the analysis: Explain the purpose of this analysis.

Pewlett Hackard is a company with a number of current employees who have already reached or will soon reach retirement age.  This "silver tsunami" of retirees places Pewlett Hackard in the difficult position of planning for the future of the company with so many of its workforce ready to retire.

### Resources
- Software: PostgreSQL 11, pgAdmin 4
- Queries: `Employee_Database_challenge.sql` (in `Queries` folder)
- Files: `retirement_titles.csv`, `unique_titles.csv`, `retiring_titles.csv`, and `mentorship_eligibility.csv` (in `Data` folder)
- Images: `mentorship_elegibility_by_title.png`, `ready_to_retire_vs_mentorship_eligible1965.png`, `mentorship_eligible_5years.png`, `ready_to_retire_vs_mentorship_eligible4years.png`, `ready_to_retire_by_dept.png` (in `Resources` folder)


## Results 

- There are 72,458 employees in the company who are reaching the age for retirement (born between Jan 1, 1952 and Dec 31, 1955)
- This is 24% of all current employees (72,458 / 300,024)
- Of those nearing retirement, 70% most (50,842 / 72,458) are Senior Engineers or Senior Staff
- The number of all current employees who are eligible for mentorship to fill the gap is 1549, of which 738 (48%) are already Senior Engineer or Senior Staff
  ![ready to retire vs eligible for mentorship](/Resources/ready_to_retire_vs_mentorship_eligible1965.png)
  


## Summary:

#### 1. How many roles will need to be filled as the "silver tsunami" begins to make an impact?
The "silver tsunami" fill most roles at the company but the majority of the roles that will need to be filled are Senior Engineer or Senior Staff (70% of ready to retire currently fill one of these two roles)

#### 2. Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
With 70% of the "silver tsunami" as Senior Staff or Senior Engineer there are enough qualified, retirement-ready employees to mentor the next generation of employees.  The real problem is that there are not enough "next generation" employees to be mentored.  The fact that there are no employees younger than 56 (born in 1965) and that no employees have been hired since 2000, is a real problem.  

The data pulled to look at those eligible for mentorship is a bit skewed as we are looking at employees born in only one year (1965), yet the group of ready to retire are looking at four years of employees.  If we expand the eligible for mentorship group to four years (born 1962 to 1965) we get a bit better idea of the numbers of employees eligible for mentorship into senior roles.

![ready to retire vs eligible for mentorship 4 years](/Resources/ready_to_retire_vs_mentorship_eligible4years.png)

This was calculated by refractoring the mentorship eligibility query

![eligible for mentorship 4 years](/Resources/mentorship_eligible_5years.png)

I was also able to look at the number of employees ready to retire by department. which showed that all departments will be facing around 11% of their work force retiring as part of the "silver tsunami"

![ready to retire by department](/Resources/ready_to_retire_by_dept.png)


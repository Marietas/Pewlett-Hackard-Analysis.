# Pewlett-Hackard-Analysis.

## Overview of the analysis

This project aims to evaluate and determine the number of retiring employees and their respective titles who would be eligible to participate in a mentorship program proposed by the Pewlett Hackard company.
To achieve this, I have used the PostgreSQL system to develop a code to complete my analysis and create a SQL Database to provide critical information such as The Number of Retiring Employees by Title and The Employees Eligible for the Mentorship Program. Therefore, this analysis will generate data supporting the manager in providing a strong recommendation to  employees closed to reach retirement age and benefit from the silver Tsunami program.
### Actual Storage Data
The current database of the company consists of six different CSV files that contain relevant employment information. The diagram below represents the current dataset and its relationship.

Fig. 1 - Diagram Actual Storage Data 

![](https://github.com/Marietas/Pewlett-Hackard-Analysis./blob/main/EmployeeDB.png)

The following query codes were written to compile and filter the information required for the analysis based on the data available:

- No. of retiring employees by title from January 1st, 1952 to December 31st, 1955

Fig. 2 - Query Code for deliverable 1

![](https://github.com/Marietas/Pewlett-Hackard-Analysis./blob/main/code%20deli-1.PNG)
The output of the code above is the generation of  three different CSV dataset: (a) retirement_titles; (b) unique_titles, and (c) retiring_titles.

- Mentorship Eligibility program for current employees born between January 1, 1965, and December 31, 1965

Fig. 3 - Query Code for deliverable 2

![](https://github.com/Marietas/Pewlett-Hackard-Analysis./blob/main/code%20deli-2.PNG)
The output of the code above is the generation of the Mentorship Eligibility dataset.

## Results

### Retiring Pewlett Hackard Employees by Titles

Based on the data generated on retiring_titles, which represent the number of employees per title born between 1952 and 1955. 

The results are presented below:

Fig. 4 - Retiring Titles summary

![](https://github.com/Marietas/Pewlett-Hackard-Analysis./blob/main/retiring_titles.PNG)

Main takeaways for this part of the analysis:
- 90,398 employees will reach the retirement age soon. 
- Nearly a third of the retirees are Senior Engineers, while another third includes the rest of the Senior Staff. 
- The total number of Senior Engineers and Senior Staff employees represents an estimated 60% of the total population.  As a result, Pewlett Hackard should prioritize these two groups to transition to retirement and initiate the process to fill out the future vacancies strategically.

### Mentorship Eligibility

The most important takeaways based on the Date of Birth as required, along with the actual positions with no closure date, are:
- 1,549 employees are eligible for the mentorship program.
- There is a higher number of employees retiring than potential mentors. This indicates that the company will need to develop an effective program to reduce the significant gap between the retiring employees and the employees who qualify as mentors. 
- There will not be managers born during 1965 who qualify for the mentorship program

Fig. 5 Mentorship Eligibility table

![](https://github.com/Marietas/Pewlett-Hackard-Analysis./blob/main/mentorship_eligibility.PNG)

## Summary

After performing this analysis, it is essential to highlight the following observations:

- The Pewlett Hackard company presents a significant number of future vacancies that will need to be filled out as soon as possible as  90,398 employees will reach retirement age in the next three years.  
- Based on the workforce available, there will only be  1,549 employees qualified to mentor new employees as part of the retirement transition.  

According to this, the company may not have enough seniors to tutor the next generation of workers, especially if we compare current potential mentors and retiring employees.  
One of the strategies to minimize this effect is to create a query code that will provide the list of retiring individuals at the end of the current year (and for each subsequent year). The company will use this information to determine the vacancies required to be filled out due to the upcoming retirements.  

In addition to the previous strategy, the developer could provide an additional query code to compare the number of retiring positions vs. eligible mentors per job title. In this way, the company will plan the workforce required for the mentorship program. 

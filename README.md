# Pewlett Hackard Employee Database Analysis

## Overview of Project

### Purpose
The purpose of this project was to take some dirty data in the form of CSV files, and upload them to a PostgreSQL server. Once our information was created within the Postgres serve, we were able to query the tables to delete duplicate entries and produce new, more concise tables for the sake of our employee retirement and mentorship eligibility tables. 

## Analysis and Challenges

### Retiring Employees
As may be expected, Pewlett Hackard is losing predominantly senior employees to retirement age. 
To produce the final count of employees retiring, we first had to create the retirement_titles table.
This was followed by using DISTINCT ON to produce our clean table of unique employee titles (or unique_titles.csv).
From there, producing our count of retiring employees (or retiring_titles.csv) was as simple as using the COUNT method on the titles in our unique_titles table. 

### Mentorship Eligibility
The mentorship_program table pulls together all current employees born in the year 1965. 
This table was built using three of the starting tables that were produced over the course of the module, and then brought together along their primary key and ordered by the employee number.
While the individual query for this table may be a more complicated block of code, it involved considerably less steps to accomplish than our retiring_titles table. 

## Summary
When the so called "silver tsunami" hits Pewlett-Hackard this year, there will be a total of 72,458 positions vacated. Of those, 50,842 employees are senior staff or engineers. 
With over 50,000 senior staff eligible for retirement and a proposed mentorship eligibility of only 1,550 employees, Pewlett Hackard is well poised to train up some of their younger staff members. 

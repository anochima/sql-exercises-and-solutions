
# Practice SQL – 10 Final Query Questions
## Exercise 1
Find the average salary of the male and female employees in each department.

## Exercise 2
Find the lowest department number encountered in the 'dept_emp' table. Then, find the highest department number.

## Exercise 3
Obtain a table containing the following three fields for all individuals whose employee number is not greater than 10040:
- employee number
- the lowest department number among the departments where the employee has worked in (Hint: use a subquery to retrieve this value from the 'dept_emp' table)
- assign '110022' as 'manager' to all individuals whose employee number is lower than or equal to 10020, and '110039' to those whose number is between 10021 and 10040 inclusive.

**Use a CASE statement to create the third field.**

If you've worked correctly, you should obtain an output containing 40 rows.

<p>Here’s the top part of the output. Does it remind you of an output you’ve obtained earlier in the course?</p>
<img src="exercise-3.png" width=200 height=200>

## Exercise 4
Retrieve a list of all employees that have been hired in 2000.

## Exercise 5
Retrieve a list of all employees from the ‘titles’ table who are engineers.
Repeat the exercise, this time retrieving a list of all employees from the ‘titles’ table who are senior
engineers.
After LIKE, you could indicate what you are looking for with or without using parentheses. Both options are
correct and will deliver the same output. We think using parentheses is better for legibility and that’s why
it is the first option we’ve suggested.

## Exercise 6
Create a procedure that asks you to insert an employee number and that will obtain an output containing
the same number, as well as the number and name of the last department the employee has worked in.
Finally, call the procedure for employee number 10010.
If you've worked correctly, you should see that employee number 10010 has worked for department
number 6 - "Quality Management".

## Exercise 7
How many contracts have been registered in the ‘salaries’ table with duration of more than one year and
of value higher than or equal to $100,000?
Hint: You may wish to compare the difference between the start and end date of the salaries contracts.

## Exercise 8
Create a trigger that checks if the hire date of an employee is higher than the current date. If true, set the
hire date to equal the current date. Format the output appropriately (YY-mm-dd).
Extra challenge: You can try to declare a new variable called 'today' which stores today's data, and then
use it in your trigger!
After creating the trigger, execute the following code to see if it's working properly.

## Exercise 9
Define a function that retrieves the largest contract salary value of an employee. Apply it to employee
number 11356.
In addition, what is the lowest contract salary value of the same employee? You may want to create a new
function that to obtain the result.

## Exercise 10
Based on the previous exercise, you can now try to create a third function that also accepts a second
parameter. Let this parameter be a character sequence. Evaluate if its value is 'min' or 'max' and based on
that retrieve either the lowest or the highest salary, respectively (using the same logic and code structure
from Exercise 9). If the inserted value is any string value different from ‘min’ or ‘max’, let the function
return the difference between the highest and the lowest salary of that employee.

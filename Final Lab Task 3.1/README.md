# Final Lab Task 3.1: Using MYSQL Clause
In this activity, querying a relational database using SQL. You will practice retrieving, grouping, and aggregating course data using SELECT statements and conditions. To analyze course enrollment details and generate insights such as fully enrolled courses, and total enrollments.

# Step 1
- Open xampp, click start to apache and mysql, and open MYSQL workbench
# Step 2
- Create database to store all data.
- Create table to organize each information.
- Code based on the instructions that has been given and execute it to see the result.
# Step 3
-  Go to Database in the left top, then click Reverse Engineer.
- Put necessary data then click next, Select your database, click next then execute and in the last part you can arrange your table based on what you want.

# Here's the screenshot of my QUERY STATEMENT and TABLE STRUCTURE
## Task 1
![screenshot](images/db.jpg)
## Task 2
![screenshot](images/courses.jpg)
## Task 3
![screenshot](images/imp.jpg)
## Task 4
TASK 1 
SELECT course_name 
FROM courses
WHERE students_enrolled<enrollment_limit;
![screenshot](images/imp.1.jpg)
## Task 5
SELECT course_name, SUM(students_enrolled) as 'total of students'
FROM courses 
GROUP BY category;
![screenshot](images/imp.2.jpg)
## Task 6
SELECT course_name 
FROM courses
WHERE students_enrolled=enrollment_limit;
![screenshot](images/imp.3.jpg)
## Task 7
SELECT SUM(students_enrolled) AS 'total number of students enrolled across all courses'
FROM courses;
![screenshot](images/imp.4.jpg)
## Task 8
SELECT course_name, students_enrolled
FROM courses 
ORDER BY students_enrolled
![screenshot](images/imp.5.jpg)

# Here's the screenshot of my ER DIAGRAM
![screenshot](images/diagram%20(2).jpg)







 







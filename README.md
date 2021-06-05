# SQL Queries

##### 1. Write an SQL query to fetch "NAME" from Student table in upper case.
```
Select upper(NAME) from Student;
```
##### 2. Write an SQL query to print the first three character of FIRST_NAME from Worker table.
```
Select substring(FIRST_NAME,1,3) from Worker;   (or)
Select left(FIRST_NAME,3) from Worker;
```
##### 3. Write an SQL query to create a empty table STUDENT_INFO from the existing table STUDENT.
```
Select * from STUDENT into STUDENT_INFO where 1=2;   (or)
Create table STUDENT_INFO as (Select *from STUDENT where 1=2);
```
##### 4. Write an SQL query to print details from Worker table with the firstname as 'Vipul' and 'Sathish'.
```
Select * from Worker where firstname = 'Vipul' or firstname = 'Sathish';   (or)
Select * from Worker where firstname in ('Vipul','Sathish');
```

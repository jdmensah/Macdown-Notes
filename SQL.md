#Introduction to SQL

* Getting data for testing 
saving data generated during testing activity 
data verifications in databases 

* Find data #
* To ensure data integrity 
* To manipulate test data for test scripts 
testing databases 

[SQL Commands ](https://www.tutorialspoint.com/sql/sql-insert-query.htm)
[SQL 2](http://g2pc1.bu.edu/~qzpeng/manual/MySQL%20Commands.htm)

* Use - Select the database you want to use 
	* use spartan_learning 

* Show - Shows tables within the database 
	* show tables in spartan_learning 

* Describe - Shows the column in the table 
	* describe people 

* Select - selects records from table 
	* select * from people 

##Aggregate functions
* count - counts all the record in the table 
	* select count(*) from people 
	* select count(*) from people where rating > 3;

* max - returns the highest value from table 
	* select max(rating) from people; 

* avg - return the average rating from the table 
	* select avg(rating) from people; 
	* select round(avg(rating), 0) from people; - *round to nearest whole number*
	* select round(avg(rating), 2) from people; - *rounds to 2 decimal places*
* sum - adds all the numeric data in the column in the table 
	* select sum(t_pay) from people; 
* having - 
```
Select department, sum(t_pay)
from people
group by department
```	  
```
select department, sum(t_pay) from people 
group by department having count(*) >1;
```
##Users & Permissions 

Create user - create a new user for the database 

```
* Create user 'guy'@'localhost'
identified by 'lovehippo810';
``` 
```
* Grant - gives users access to database and table 
	* grant all privileges 
	on spartan_learning.people
	to 'joe'@'localhost';

```

```
select * from books where author_id = 
(select author_id from authors where author_name = "Hannah Arendt");

```

```
* drop user 'joe'@'localhost'
	* drop user 'joe'@'localhost';
```

##Inner Joins 

```
select * from employees
inner join departments
on employees.department_id=departments.id;
```
###Two inner joins 
```
select books.isbn as 'ISBN' ,a.author_name as 'Author', p.publisher as 'Publisher', books.pub_year as 'Publication Year', books.title as 'Book Title', p.pub_address as 'Publication Address'
from books
inner join authors a
on a.author_id=books.author_id
inner join publishers p
on p.pub_id=books.pub_id
```
##Aliases 
```
select * from employees as e, departments as d 
where e.department_id=d.id;

or 

select * from employees e, departments d 
where e.department_id=d.id;

```
##Outer Joins 
**Left Outer Joins**

Map the *from table* to the *join table*

```
Select * from employees 
Left out join departments 
on employees.department_id = department.id
```

**Right Outer Join** 

map the *table in the join* to the *from table* 

```
Select * from employees 
right out join departments 
on employees.department_id = department.id 
```

#Subqueries

```
select * 
from books 
where author_id = 
(select author_id from authors where author_name = "Hannah Arendt");
```

select * from people where t_pay > (select avg(t_pay)
#Joins vs Subqueries 
Joints are more performant 
joins are more powerful 
subqueries are easier to read 
subqueries are good for aggregate functions 

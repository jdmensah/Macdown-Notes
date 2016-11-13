#Introduction To Databases 

##What's a Database
A place to store information in a structured way.  

A record encapsulates data 
a record is an entity 
each column is an attribute

##Types of Database
###Documents 

* MogoDB
* Elasticsearch

###Key Value Datastore 

* Redis 
* Memcached 

###Relational Database 

* SQLite 
* MySQL

##Terminology

* Column - Database tables are composed of individual columns corresponding to the attributes of the object 
* Row - A row consists of one set of attributes corresponding to one instance that a table describes. also know as records  
* Field - a field is a single unit of data stored as part of database record. Fields are often also referred to as attributes 
* Table - a is predefined format of rows and columns  
* DBMS

##Relations
 
* One to one - each row in table a is linked to another row 
* One-to-many - 
* Many-to-many -

##Primary Key Constraints 

* Uniquely identifies each record 
* Must be unique
* Cannot be empty, black or NULL
* value can never change 
* Two Types: 
	* Single 
	* Compound 

##Foreign Keys 

* Natural relationships exist between tables in most database structures, foreign keys are used to create solid relationships
* There is no uniqueness constraint to foreign keys 
* A table can have any number of foreign.

![Hypothetical Relational Database Model](http://www.ibm.com/developerworks/library/x-matters8/relat.gif)

## Entity Relationship Diagram - ERD

* User log in regularly and complete their timesheet
* Each week they have to submit the weeks timesheet to their manager by clicking a submit button 
* A manager can add projects and work types and authorise timesheet for people who they manage 
* Thus the CEO is the only person who can authorise everyones sheets is the CEO
 
![ERD Assignment](/Users/JST/Downloads/WhatsApp Image 2016-10-25 at 11.31.59.jpeg)



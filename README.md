# SQL-for-Data-Science : Data Models
Personal Resources from the UCDavis course by Sadie St. Lawrence
------------------------------------------------------------------------------

Why is thinking before coding important?
1. Think before you do. Ask yourself – What is the problem you’re trying to solve?
2. Understand your data
  a. Understand your business process/ subject matter the data is modelled after and know the business rules
  b. Understand how your data is organised and structured in the table (how it is modelled)
    i. How the data relates to each other
    ii. How to join the data
    iii. Number and purpose of columns
3. Importance:
  a. Get more accurate results
  b. Speed up your work and reduce rework



What is a database?
1. Database: A container (a file or a set of files) to store organised data, a set of related information. (like a wall of cabinets)
2. Table: A structured list of data elements or specific data types within a database. (a single cabinet)
3. Columns: A single field in a table.
4. Row: A record in a table.



What is Data Modelling?
1. Data Modelling is a way to organise and structure information into multiple related tables and analyse how they relate to each other (data analysis).
2. A data model should always closely represent a real world problem. It can represent a business process or show the relationship between business processes.
3. Data models are data tables represented and organised in a database. They are different from models of prediction built by data scientists.



Evolution of data models
1. Relational
  a. Simplifies connection between data
  b. Easily allows you to write queries against it, retrieve it, update and write data to it.
2. NoSQL
  a. Part of the Big Data Movement
  b. Popularly called ‘Not Only SQL’
  c. It is a mechanism for storage and retrieval of unstructured data modelled by means other than tabular relations in relational databases.



What is the difference between Relational Models and Transactional Models?
	1. Relational Models:
  a. Shows relationships between different tables
  b. Allows for easy querying and data manipulation in an easy, logical and intuitive way
  c. Benefits:
    i. Efficient storage
    ii. Easier manipulation
    iii. Greater scalability
    iv.	Logically models a business process	
2. Transactional Models:
  a. Similar to an Operational Database. E.g.- storing insurance claims within a healthcare database
  b. Not easy. Usually data needs to be extracted and stored in a relational database.



Data Model Building Blocks
1. Entity
  a. Person, place, thing or event
  b. Distinguishable, unique and distinct
2. Attributes: Characteristics of an entity
3. Relationships
  a. Describes association among different entities
  b. Types:
    i. One-to-Many (e.g.- customer to invoices)
    ii. Many-to-Many (e.g.- student to classes)
    iii. One-to-One (e.g.- manager to store)



What is the difference between Primary Keys and Foreign Keys?

Primary Keys: A column or set of columns whose values uniquely identify every row in a table	
Foreign Keys: One or more columns that can be used together to identify a single row in another table
Similarities:
1. Used to join tables together
2. Prevents duplication of data in multiple tables



ER Diagrams

1. An ER model is composed of entity types and specifies relationships that can exist between instances of those entity types
2. Represented visually
3. Shows relationships and links(primary keys) between tables
4. Helps to represent a business process
5. Examples:
  a. Chen Notation
  b. Crow's Foot Notation
  c. UML Class Diagram Notation

 


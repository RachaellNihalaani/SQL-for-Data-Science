# SQL-for-Data-Science : Tables
Personal Resources from the UCDavis course by Sadie St. Lawrence

## Why are tables useful?
1. Tables are used to make models and predictions
2. Create dashboards
3. Visualise data with other tools
4. Extract data from other sources

### Query to create a table:
*CREATE TABLE table_name
(
  column_name1	datatype(limit)	specification,
	column_name2	datatype(limit)	specification,
	column_name3	datatype(limit)	specification,
);*

E.g. - 			char(10)		PRIMARY KEY,
				decimal(8,2)	NOT NULL,



## Nulls and Primary Key
1. Every column is either NULL (default) or NOT NULL
2. If a column is specified to be NOT NULL, then an error is returned if one tries to submit no value
3. Null Value (NULL – absence of everything) is not the same as an Empty String (“  ” – string of spaces etc.)
4. Primary keys cannot be NULL. They must have a value.



### Query to add data to the table:
*INSERT INTO table_name
VALUES (  ‘value1’ 
               , ‘value2’ 
               , ‘value3’ 
                              );*
Or
*INSERT INTO table_name (‘column1’ 
                                           , ‘column2’ 
                                            , ‘column3’ 
                                                             );
VALUES (  ‘value1’ 
               , ‘value2’ 
               , ‘value3’ 
                              );*



## Creating Temporary Tables
1. Will be deleted when the current session is terminated
2. Faster than creating a real table
3. Useful for complex queries using subsets/ copies of other tables and joining them



### Query to create a temporary table:
*CREATE TEMPORARY TABLE temp_table_name AS
(		
	SELECT *
	FROM table_name
	WHERE column_name = ‘value’
);*



## Retrieving Data with SELECT Statement
### Query for retrieving a single column:
*SELECT column_name
FROM table_name;*

### Query for retrieving multiple columns:
*SELECT column_name1, column_name2, column_name3
FROM table_name;
Or
SELECT column_name1
, column_name2
, column_name3
FROM table_name;*

### Query for retrieving all columns:
*SELECT *
FROM table_name;*

### Query for limiting the amount of data returned:
In SQLite:
*SELECT column_name(s)
FROM table_name
LIMIT number_of_records;*

In Oracle:
*SELECT column_name(s)
FROM table_name
WHERE ROWNUM<=N;*

In DB2:
*SELECT column_name(s)
FROM table_name
FETCH FIRST N ROWS ONLY;*

Reason to limit amount of data returned: If database is large and you only want to see a sample of the data, it will return only first N records.

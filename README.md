# Project-14-SQL-commands-PostgreSQL
These are assignments given in Patika Java Intermediate course.

The tasks are:

* List the top 5 longest films (by length) in the film table where the film title (title) ends with the letter 'n'.
* List the next 5 shortest films (6th, 7th, 8th, 9th, and 10th) in the film table where the film title (title) ends with the letter 'n'.
* List the top 4 records from the customer table, ordered by last_name in descending order, where store_id is 1.


## The Queries 

```

-- Task1
SELECT * FROM film 
WHERE title LIKE '%n' 
ORDER BY length DESC
LIMIT 5;

-- Task 2
SELECT * FROM film 
WHERE title LIKE '%n' 
ORDER BY length 
OFFSET 5
LIMIT 5;

-- Task 3
SELECT * FROM customer 
WHERE store_id = 1
ORDER BY last_name DESC 
LIMIT 4;
```
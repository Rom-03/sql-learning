# My SQL Learning Journey — Week 1

Hi everyone! 👋 
This past week, I committed myself to learning SQL from scratch — and I'm excited to share what I've accomplished so far. This post serves as both a milestone and a reference for anyone else just getting started.

---

## What I Learned

### SQL Basics
- Understood what SQL is and how it's used to manage data
- Used `SELECT` and `FROM` to retrieve data from tables

SELECT * FROM users;
SELECT name, age FROM users;

---

### Creating Tables and Inserting Data

Before running queries, I created a sample table called `users` and inserted some example records to work with.

```sql
-- Create a table named 'users'
CREATE TABLE users (
    id INT PRIMARY KEY,
    name VARCHAR(50),
    age INT,
    city VARCHAR (50)
);

-- Insert sample data
INSERT INTO users (id, name, age, city) VALUES
(1,'Anna',23,'Manila'),
(2,'Brian',31,'Cebu'),
(3,'Carla',28,'Davao'),
(4,'Daniel',19,'Manila'),
(5,'Elain',35,'Cebu');

```

🔸 Filtering Data
	•	Applied filters using the WHERE clause with comparison operators like =, <, >, !=

```sql
SELECT * FROM users WHERE city = 'Cebu';
SELECT name, age FROM users WHERE age > 25;

```

🔸 Logical Conditions
	•	Combined multiple conditions with AND, OR, and NOT

```sql
SELECT * FROM users WHERE age > 25 AND city = 'Cebu';
SELECT * FROM users WHERE city = 'Davao' OR age < 25;

```

🔸 Sorting and Limiting Results
	•	Used ORDER BY to sort results ascending or descending
	•	Applied LIMIT to return only a subset of rows

```sql
SELECT * FROM users ORDER BY age DESC;
SELECT * FROM users ORDER BY age ASC LIMIT 2;

```

🔸 Pattern Matching and List Filtering
	•	Used LIKE with % to match text patterns
	•	Used IN to filter from a list of values
	•	Used BETWEEN to filter numeric ranges

```sql
SELECT name FROM users WHERE name LIKE '%a';
SELECT * FROM users WHERE city IN ('Manila', 'Cebu');
SELECT * FROM users WHERE age BETWEEN 25 AND 35;

```

🔸 Aggregate Functions
	•	Learned how to summarize data with built-in SQL functions

```sql
SELECT COUNT(*) FROM users;
SELECT AVG(age) FROM users;
SELECT SUM(age) FROM users;
SELECT MIN(age), MAX(age) FROM users;

```

🔸 Mini Challenges and Practice

Wrote and solved several SQL scenarios, such as:

✅ Count users per city

✅ Filter names ending in “a”

✅ Get top 3 oldest users

✅ Calculate average age

✅ Show youngest and oldest users

```sql
SELECT city, COUNT(*) AS user_count
FROM users
GROUP BY city;

SELECT * FROM users WHERE name LIKE '%a';
SELECT name, age FROM users ORDER BY age DESC LIMIT 3;
SELECT AVG(age) FROM users;
SELECT MIN(age), MAX(age) FROM users;

```
### Key Takeaways

•	I’m now comfortable with basic querying, filtering, sorting, and summarizing data in SQL
•	SQL syntax is readable and powerful — it’s a must-have skill for any IT or data-related role
•	Practice makes concepts stick — daily activities helped a lot!

### What’s Next?

Next week I’ll dive into:
	•	GROUP BY + HAVING
	•	SQL JOINs (Inner, Left, Right)
	•	Subqueries
	•	Modifying data with INSERT, UPDATE, and DELETE

 
 

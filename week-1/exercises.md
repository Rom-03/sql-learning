# My Questions and Activities on Week 1

This section contains all the questions and exercises I completed during Week 1 of learning SQL. These helped reinforce my understanding of core SQL concepts like creating tables, filtering data, sorting, and using aggregate functions.

---

### Table Creation and Data Insertion

**Q1.** Write a SQL command to create a `users` table with the following fields:
- `id` (integer, primary key)
- `name` (string)
- `age` (integer)
- `city` (string)

<details><summary>Answer</summary>

```sql
CREATE TABLE users (
    id INT PRIMARY KEY,
    name VARCHAR(50),
    age INT,
    city VARCHAR(50)
);
```
</details>

## Q2. Insert the following data into the users table:

| id | name   | age | city   |
|----|--------|-----|--------|
| 1  | Anna   | 23  | Manila |
| 2  | Brian  | 31  | Cebu   |
| 3  | Carla  | 29  | Davao  |
| 4  | Daniel | 19  | Manila |
| 5  | Elain  | 35  | Cebu   |


<details><summary>Answer</summary>

```sql
INSERT INTO users (id, name, age, city) VALUES
(1, 'Anna', 23, 'Manila'),
(2, 'Brian', 31, 'Cebu'),
(3, 'Carla', 29, 'Davao'),
(4, 'Daniel', 19, 'Manila'),
(5, 'Elain', 35, 'Cebu');

```
</details>

### Try It Yourself

- [One Compiler](https://onecompiler.com)

## SELECT, WHERE, AND/OR

Q3. Show all users in the table.

Q4. Show names and ages of users who live in Cebu.

Q5. Show users older than 30.

Q6. Show users younger than 30 AND from Manila.

Q7. Show users who live in Davao OR are younger than 25.

## LIKE, IN, BETWEEN

Q8. Show users whose name ends with the letter “a”.

Q9. Show users from either Cebu or Davao.

Q10. Show users aged between 25 and 35.

⸻

## ORDER BY, LIMIT

Q11. List all users sorted by age in descending order.
Q12. Show the top 3 oldest users.
Q13. Show the youngest user.

⸻

## Aggregate Functions

Q14. How many users are in the table?

Q15. What is the average age of users?

Q16. What is the sum of all users’ ages?

Q17. Show the youngest and oldest user ages.

Q18. Count how many users live in each city.


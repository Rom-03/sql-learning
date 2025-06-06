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



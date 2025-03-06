## 0. Convert this table data into json data

```sql
CREATE TABLE Employees (
employee_id INT PRIMARY KEY,
first_name VARCHAR(50),
last_name VARCHAR(50),
department VARCHAR(50),
salary INT
);

INSERT INTO Employees VALUES (1, 'Hakan', 'Hakansson', 'HR', 30000);
INSERT INTO Employees VALUES (2, 'Bob', 'Bobson', 'IT', 35000);
```

### a) Start with writing out the table with the data

Employees

| employee_id | first_name | last_name | department | salary |
| ----------- | ---------- | --------- | ---------- | ------ |
| 1           | Hakan      | Hakansson | HR         | 30000  |
| 2           | Bob        | Bobsson   | IT         | 35000  |

### b) Manually convert data into semi-structured JSON format.

```json
{
  "employees": [
    {
      "employee_id": 1,
      "first_name": "Hakan",
      "last_name": "Hakansson",
      "department": "HR",
      "salary": 30000
    },
    {
      "employee_id": 2,
      "first_name": "Bob",
      "last_name": "Bobsson",
      "department": "IT",
      "salary": 35000
    }
  ]
}
```

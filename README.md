# sql-payment-analysis
MySQL project demonstrating database creation, data insertion, GROUP BY, and COUNT aggregate functions to analyze customer payment methods.
# Customer Payment Method Analysis (MySQL)

## Project Overview

This project demonstrates basic SQL operations using MySQL. It focuses on analyzing customer payment methods using the GROUP BY clause and COUNT() aggregate function.

The project contains 10 customer records and categorizes them based on their payment methods.

## Database Information

| Property | Details |
|---|---|
| Database Name | `consumer` |
| Table Name | `payment` |
| Total Records | 10 |
| Database Tool | MySQL |
| IDE | MySQL Workbench |

## Table Structure

| Column Name | Data Type | Constraints |
|---|---|---|
| customer_id | INT | PRIMARY KEY |
| customer | VARCHAR(50) | NOT NULL |
| mode | VARCHAR(20) | NOT NULL |
| city | VARCHAR(20) | NOT NULL |

## SQL Concepts Used

| SQL Concept | Purpose |
|---|---|
| CREATE DATABASE | Creates the database |
| USE | Selects the database |
| CREATE TABLE | Creates the payment table |
| PRIMARY KEY | Ensures unique customer IDs |
| NOT NULL | Prevents empty values |
| INSERT INTO | Inserts customer records |
| SELECT | Retrieves data |
| COUNT() | Counts customers |
| GROUP BY | Groups customers by payment method |

## Analysis Query

```sql
SELECT mode, COUNT(customer)
FROM payment
GROUP BY mode;
```

## Query Results

| Payment Method | Number of Customers |
|---|---:|
| Netbanking | 4 |
| Credit Card | 4 |
| Debit Card | 2 |
| **Total** | **10** |

## Key Findings

- Netbanking is used by 4 customers.
- Credit Card is used by 4 customers.
- Debit Card is used by 2 customers.
- Netbanking and Credit Card are equally common in this dataset.

## Repository File Structure

```text
sql-payment-analysis/
│
├── README.md
├── payment_analysis.sql
│
└── screenshots/
    ├── sql_code.png
    └── query_output.png
```

| File / Folder | Description |
|---|---|
| `README.md` | Project documentation |
| `payment_analysis.sql` | Complete SQL script |
| `screenshots/` | Project screenshots |
| `sql_code.png` | SQL code screenshot |
| `query_output.png` | Query result screenshot |


## How to Run

1. Open MySQL Workbench.
2. Open `payment_analysis.sql`.
3. Execute the SQL script.
4. Run the GROUP BY query.
5. View the results in the Result Grid.

## Tools Used

| Tool | Purpose |
|---|---|
| MySQL | Database management |
| MySQL Workbench | SQL development |
| GitHub | Project hosting |

## Learning Outcomes

- Learned to create databases and tables.
- Practiced inserting multiple records.
- Understood aggregate functions.
- Learned how to use GROUP BY.
- Analyzed customer payment preferences using SQL.

---

**Author:** Sameer

**Project Type:** Beginner SQL Data Analysis Project

# Grocery Sales Analysis with SQL

Category-level sales performance analysis on a grocery dataset using SQL in Google BigQuery. This project is part of the RevoU Full Stack Data Analytics assignment.

## Dataset

Dataset: `fsda-sql-01.grocery_dataset`

| Table | Description |
|---|---|
| `sales` | Transaction data (customer, product, quantity, discount, date, transaction number) |
| `products` | Product data (price, category) |
| `categories` | Product category names |

## Analyses

| No | Analysis | SQL Techniques |
|---|---|---|
| 1 | Revenue after discount by category | JOIN, SUM, GROUP BY |
| 2 | Total units sold and revenue by category | JOIN, SUM |
| 3 | Unique customers and revenue by category | COUNT DISTINCT |
| 4 | Average price per unit by category | AVG |
| 5 | Average price vs. unique buyers comparison | CTE, joining CTEs |
| 6 | Revenue contribution per category (%) | CTE, Window Function `SUM() OVER ()` |
| 7 | Repeat purchase rate by category | CTE, CASE WHEN |
| 8 | Category metrics summary (units, customers, revenue, contribution) | CTE, Window Function |
| 9 | Cumulative transactions of the top-spending customer | CTE, Running Total `ROWS BETWEEN` |

## Revenue Formula

```
revenue_after_discount = quantity × price × (1 − discount)
```

## Repository Structure

```
grocery-sales-analysis-sql/
├── grocery_analysis.sql
└── README.md
```

## How to Run

1. Open the Google BigQuery Console.
2. Make sure you have access to the `fsda-sql-01.grocery_dataset` dataset.
3. Copy the queries from `grocery_analysis.sql` and run them one by one.

## Tools

Google BigQuery (Standard SQL)

## Author

**Rei** ([@ReinaldyZA](https://github.com/ReinaldyZA))

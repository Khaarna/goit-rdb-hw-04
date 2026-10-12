# Relational Databases — Homework 4

## Dataset

**Name:** Olist Brazilian E-Commerce Public Dataset

**Source:** [Kaggle — Olist Brazilian E-Commerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

The dataset contains information about approximately 100,000 orders placed on a Brazilian e-commerce platform between 2016 and 2018.

For this homework, six CSV files were used:

| Table | Records |
|---|---:|
| Customers | 99,441 |
| Orders | 99,441 |
| Order Items | 112,650 |
| Products | 32,951 |
| Sellers | 3,095 |
| Order Reviews | 99,224 |

The complete datasets were used without sampling.

## Tools

- Google Colab
- PostgreSQL 16 (`pgserver`)
- Python
- SQLAlchemy
- pandas
- KaggleHub

## Homework Tasks

The following tasks were completed:

1. **Data Loading and DDL** — Downloaded the Olist dataset, created raw and typed tables with primary keys, foreign keys, and constraints.
2. **DML Operations** — Used `INSERT ... RETURNING`, `ON CONFLICT`, `UPDATE ... FROM`, and `DELETE ... RETURNING`.
3. **Customer Segmentation** — Created customer-level segments using purchase frequency, total spending, and recency.
4. **JOIN Queries** — Practiced `INNER JOIN`, `LEFT JOIN`, `FULL OUTER JOIN`, `SELF JOIN`, and anti-join.
5. **Aggregations** — Calculated seller ratings, product category sales, and seller statistics using `GROUP BY`, `HAVING`, and `STRING_AGG`.
6. **Advanced SQL** — Used `INTERSECT`, `EXCEPT`, `UNION ALL`, CTEs, and the `DENSE_RANK()` window function.
7. **Reflection** — Summarized the main challenges and decisions related to database design and data analysis.

## Results

- Created six raw and six typed tables.
- Identified 96,096 unique customers using `customer_unique_id`.
- Divided customers into four segments: VIP, regular, new, and inactive.
- Calculated seller ratings without duplicating reviews from multi-item orders.
- Analyzed orders, products, sellers, and customer behavior using SQL.

## How to Run

1. Open `HW04.ipynb` in Google Colab.
2. Select **Runtime → Restart session and run all**.
3. Wait for all cells to finish executing.

The notebook automatically installs dependencies, downloads the Olist dataset using KaggleHub, starts PostgreSQL, creates tables, and executes SQL queries.

No manual database setup is required.

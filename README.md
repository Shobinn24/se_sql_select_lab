# SQL Select Lab 🗄️

A Python lab exploring SQL fundamentals using SQLite and Pandas, built as part of the Flatiron School Full Stack Software Engineering program.

## Project Description

This lab simulates working as a data specialist in the HR department of the fictional Northwinds Company. Using SQL queries through Python, I retrieved and transformed employee and order data stored in a SQLite database. The project covers core SQL concepts including filtering, aliasing, CASE statements, and built-in string/numeric/date functions.

## Technologies Used

- **Python 3.11**
- **SQLite3** — built-in Python library for connecting to SQL databases
- **Pandas** — for loading SQL query results into DataFrames
- **Pytest** — for running the test suite

## How to Run It

**1. Clone the repository**
```bash
git clone https://github.com/Shobinn24/se_sql_select_lab
cd se_sql_select_lab
```

**2. Install dependencies**
```bash
pip3 install pandas pytest
```

**3. Run the test suite**
```bash
python3 -m pytest ./test_main.py
```

**4. Run the main file directly**
```bash
python3 main.py
```

## What I Learned

**SQL Querying with Python**
Connecting a SQLite database to Python using `sqlite3` and loading query results directly into Pandas DataFrames with `pd.read_sql()`.

**SELECT & Filtering**
Selecting specific columns instead of `SELECT *`, and controlling column order in the output.

**Aliasing with AS**
Renaming columns in query results using `AS` for cleaner, more readable output.

**CASE Statements**
Using `CASE WHEN ... THEN ... ELSE ... END` as SQL's version of if/elif/else to create new categorization columns on the fly.

**Built-in SQL Functions**
- `LENGTH()` — get the character length of a string
- `SUBSTR()` — extract a substring (note: SQL uses 1-based indexing, unlike Python)
- `ROUND()` and `SUM()` — numeric operations on query results
- `STRFTIME()` — extract day, month, and year from date columns

**Debugging Database Issues**
Learned to inspect actual table schemas and column names using `SELECT * FROM table LIMIT 1` when queries fail, rather than assuming column names match documentation.

**Python Environment Management**
Worked through `pipenv` and Python version conflicts, ultimately resolving dependency issues by installing packages with `pip3` and running tests with `python3 -m pytest`.

## Test Results

```
9 passed in 0.47s ✅
```
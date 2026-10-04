Task 15 — Pandas DataFrame Basics

## 1. Project Overview
This task introduces the Pandas DataFrame, the primary Pandas structure used for tabular data analysis. A DataFrame stores information in rows and columns, similar to a spreadsheet or database table.

## 2. Objective
Learn how to create, load, inspect, select, filter, and summarize tabular data using Pandas DataFrames.

## 3. Tools
- Python
- Pandas
- Jupyter Notebook

## 4. Deliverables
- Create a DataFrame manually.
- Load a real CSV dataset into a DataFrame.
- Explore rows and columns.
- Display shape, column names, and data types.
- Use `head()`, `tail()`, and `info()`.
- Use `describe()` for numerical summaries.
- Perform practical filtering and student-performance analysis.

## 5. Main Concepts

DataFrame
A two-dimensional labeled data structure containing rows and columns.

`pd.DataFrame()`
Creates a DataFrame from dictionaries, lists, arrays, or similar structured data.

`pd.read_csv()`
Loads CSV data into a DataFrame.

`head()` and `tail()`
Quickly inspect the beginning and end of a dataset.

`shape`
Returns `(number_of_rows, number_of_columns)`.

`columns`
Returns the column labels.

`dtypes`
Shows the data type of every column.

`info()`
Provides a structural summary including columns, non-null counts, and data types.

`describe()`
Provides descriptive statistics for numerical columns.

Boolean filtering
Selects rows that satisfy a condition, such as:
```python
df[df["Average"] >= 80]
```

Missing-value check
```python
df.isnull().sum()
```
counts missing values in each column.

## 6. Practical Workflow
Load → Inspect → Check shape/types → Check missing values → Select columns → Filter rows → Calculate statistics → Interpret results.

## 7. Dataset
`student_performance.csv` contains student IDs, names, ages, Python marks, SQL marks, attendance, average marks, and performance categories.

## 8. Run
```bash
pip install pandas jupyter
python Task_15.py
jupyter notebook Task_15.ipynb
```

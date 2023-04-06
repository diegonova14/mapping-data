# Mapping Data in Python
Coursera Lesson 2: Mapping Data to Python

This was a proposed exercise in Coursera course: [Python, Bash and SQL Essentials for Data Engineering Specialization](https://www.coursera.org/specializations/python-bash-sql-data-engineering-duke) that covers the following topics:

1. Develop data engineering solutions using Python and the Linux environment
2. Design scripts to connect and query a SQL database using Python
3. Use a scraping tool to extract data from the web
4. Setup a provisioned Python project environment

## Exercise
For this exercise, I will be using data from the [sample_data/](/sample_data) and the [exercise.ipynb](/exercise.ipynb) notebook.

## What did I do?
This exercise is solved in [practice.ipynb](/practice.ipynb) file.
The objetive is to retrieven Italian red and white wines which were rated between 90 and 92 ina a json file.

To achieve this I used the library pandas.

I imported the data using the function:
```
read_json()
```
Then, I verified the available varieties if it was worthy to filtering since there were more than red and white wines.

The next step was to filter all rows which contained 'Red wine' or 'White wine' and were stored in `wines_rw`, which in turn was filtered by rating between 90 and 92 and stored in `wines_score`.

Finally, `wines_score` was filtered by wines, whose region of origin contained the word "Italy".

The json export was made using the function:
```
to_json()
```
and saved in [sample_data/](/sample_data) directory.
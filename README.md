# Movies-ETL
Clean and organize movie data by creating a pipeline that takes new data, performs appropriate transformations, and loads the data into existing tables using pandas library and python in jupyter notebook and PostgreSQL database to store the tables.

## Overview
With knowledge of writing code to perform an ETL on given data, we will write an ETL function to read three data files (CSV and JSON) then extract and transform the wikipedia and kaggle data. Finally, we will create the movie database in PostgreSQL.

## Results
Using Python, Pandas, ETL, and code refactoring:
- we have written a function that reads in the three data files and creates three separate DataFrames. To view the DataFrames, see the file ETL_function_test.ipynb in the repository.
- we merged the Wikipedia and Kaggle metadata by extracting and transforming the Wikipedia data. To view the merged DataFrame, see the file ETL_clean_wiki_movies.ipynb in the repo.
- we extracted and transformed the Kaggle metadata and MovieLens rating data. Then, by converting the data into separate DataFrames, we merge the Kaggle metadata DataFrame with the Wikipedia movies DataFrame and the MovieLens rating data. With this organization and combination of data, all movie data can be viewed in one DataFrame including movies with their ratings. To view these DataFrames, see the file ETL_clean_kaggle_data.ipynb in the repo.
- the movies DataFrame and MovieLens rating CSV data are in a SQL database

# Overview
The Wedge is a Minneapolis Co-op that provided data to our professor for use in this exercise. The data was provided in the form of over 50 CSV files zipped in different formats. This presented a challenge in taking the data from its raw form, to a cleaned and usable Pandas dataframe, to Google Big Query for analysis, and finally a local SQL database. The project was split into three tasks. I will provide more detail on each individual task below.

# Task 1
In this task, I read in 53 zipped data files with differing delimiters, heaters, and datatypes. After unzipping, the code in the notebook corrects delimiters, normalizes datatypes, fixes issues with headers, and deals with null values. Once the data has been cleaned, it is converted into a pandas dataframe and uploaded to Google Big Query in preparation for analysis in later stages of the project.

# Task 2
In this task, I connect to the data uploaded to Google Big Query in the previous part of the project. I then use pandas_gbq to query the data and pull a random sample of Card Number owners in the data, as well as all records involving them. I used a CTE to get the sample, and pulled records within the same query. To conclude this task, the code converts the query result to a pandas dataframe, and writes that dataframe to a CSV file output.

# Task 3
In this task, I was asked to create a local SQL database from the Google Big Query data previously uploaded. In order to accomplish this, I created 3 GBQ queries to meet the requirements for the database. The GBQ queries are as follows: Sales by date and hour, Sales by owner, year, and month, and Sales by product description. Upon successful completion of these queries, the results were saved in CSV format on my machine. I then established a SQLite3 connection and created an empty database. This was followed by uploading the CSV files as tables in the database. The resulting database matches the requirements of the project.

# Results
This project was graded as successful completion at the grade requirements for an A.



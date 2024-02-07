# Overview
The Wedge is a Minneapolis Co-op that provided data to our professor for use in this exercise. The data was provided in the form of over 50 CSV files zipped in different formats. This presented a challenge in taking the data from its raw form, to a cleaned and usable Pandas dataframe, to Google Big Query for analysis, and finally a local SQL database. The project was split into three tasks. I will provide more detail on each individual task below.

# Task 1
In this task, I read in 53 zipped data files with differing delimiters, heaters, and datatypes. After unzipping, the code in the notebook corrects delimiters, normalizes datatypes, fixes issues with headers, and deals with null values. Once the data has been cleaned, it is converted into a pandas dataframe and uploaded to Google Big Query in preparation for analysis in later stages of the project.

# Task 2
In this task, I connect to the data uploaded to Google Big Query in the previous part of the project. I then use pandas_gbq to query the data and pull a random sample of Card Number owners in the data, as well as all records involving them. I used a CTE to get the sample, and pulled records within the same query. To conclude this task, the code converts the query result to a pandas dataframe, and writes that dataframe to a CSV file output.

# Task 3



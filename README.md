# Home_Sales

An analysis conducted in a jupyter notbook that uses PySparkSQL to determine key metrics about home sales data stored in a big data cloud storage provider.

## Description

Cloud storage services such as AWS, Google Cloud, and Azure allow for the storage and access of very large data files that may be more than a traditional database can handle.  Combined with tools such as PySparkSQL, big data can be stored, manipulated, and queried much more efficiently and at faster rates depending on how the data is structured and partitioned.

This analysis is meant to demonstrate how cloud storage and PySparkSQL can be used to this end by analyzing a large data set of home sales and answering the following questions:

1. What is the average price for a four-bedroom house sold for each year?
2. What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms?
3. What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet?
4. What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000?

In addition to answering the above questions, this analysis also takes a look at performance by comparing the runtime of completeing the last query when the data is uncached, chached, and partitioned by a specific field ('date_built') in a formatted parquet.

### Dependencies
* Python / Jupyter Notebook
* findspark
* pyspark.sql
* Internet connection to access data file in cloud storage

### Installing & Execution
The file 'Home_Sales.ipynb' can be downloaded and executed.  Note that since the file references a data file stored in a cloud storage provider (AWS), an internet connection is necessary to properly run the file.

## Authors

Daniel Pineda

## Acknowledgments
Home_Sales was created as an assignment for the University of California, Irvine Data Analytics Bootcamp - June 2024 Cohort under the instruction and guidance of Melissa Engle (Instructor) and Mitchell Stone (TA).
The practical exercises and coding examples demonstrated through the bootcamp helped inform and inspire the code for this project.
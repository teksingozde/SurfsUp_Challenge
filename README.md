# SurfsUp Challenge

## Overview of Project
A study is being conducted on the investor who wants to establish a surf-based business in Hawaii, wanting to learn about the feasibility of the business in this region. In order to establish a surf-based business in this region, the climate must be favorable, and the study includes data on the climate of the Hawaiian region.

## Resources
### Datasets:
- climate_analysis.ipynb
- hawaii.sqlite

### Software: 
- Python 3. 9. 12
- Jupyter Notebook 6. 4. 8
- Pandas 1. 4. 2
- Numpy 1. 21. 5
- SQLAlchemy 1. 4. 32
- Flask 1. 1. 2

## Overview of the Analysis 
We agree that the data should be stored in an SQLite file. For this reason, we should also mention that we use SQLAlchemy so that we can access and analyze. In order for us to analyze, connecting to the database is the first priority, and for this we create an engine that we call the engine. With the help of this engine, an installation is made to connect Python to the database.

First of all, we need to talk about the Flask application. In order to start the Flask application, a SQLite database is being prepared with the SQLAlchemy library.

After the initialization process, the URL was added and SQLAlchemy was used to get the precipitation data measured between 23 August 2016 and 23 August 2017. Afterwards, it was frozen as a JSON object again using SQAlchemy and a station was created here. Afterwards, a situation occurs where the start date is obligatory and the end date is at the discretion of the user. Here, you can have information about the minimum and maximum temperatures and the average observed temperatures between dates.
The months we are asked to analyze are July and December. Necessary tables and explanations are included in the results section.

## Results
#### Table 1. June Temperatures
<img width="131" alt="Screen Shot 2022-11-08 at 10 47 54 PM" src="https://user-images.githubusercontent.com/26927158/201194105-6adeb532-13a8-4d3b-b987-b0f78750a071.png">

First of all, some of the temperatures for June are shown in Table 1. It is observed that in the first 10 lines the lowest temperature among these temperatures is 76 degrees according to the data in the table. The highest temperature is 79 degrees according to the data in the table.

#### Table 2. December Temperatures
<img width="156" alt="Screen Shot 2022-11-08 at 10 48 30 PM" src="https://user-images.githubusercontent.com/26927158/201194472-f4c49083-e7f6-4b28-b19c-9234f47e46fe.png">

The table showing the temperatures for December is as above. According to the information above, the lowest temperature in the first 10 lines is 64 degrees, while the highest temperature is 77 degrees. However, when looking at the table in general, it can be interpreted that the temperatures suddenly drop and rise.

#### Table 3. June Temperature Statistics
<img width="158" alt="Screen Shot 2022-11-08 at 10 48 16 PM" src="https://user-images.githubusercontent.com/26927158/201194712-919cbef2-1b8f-4add-b751-5f95d7de190d.png">

We have seen the temperatures of the first 10 rows of June data in table 1. Looking at the month of June in general,
- average temperature 75,
- standard deviation 3.25,
- minimum measured temperature degree 64,
- the maximum measured temperature is 85 degree. 

#### Table 4. December Temperature Statistics
<img width="176" alt="Screen Shot 2022-11-08 at 10 48 42 PM" src="https://user-images.githubusercontent.com/26927158/201194813-e6260089-1e64-40e2-ae56-5f09618782c0.png">

We have seen the temperatures of the first 10 rows of June data in table 2. Looking at the month of December in general,
- average temperature 71,
- standard deviation 3.74,
- minimum measured temperature degree 56,
- the maximum measured temperature is 83 degrees.

## Summary

In general, when the statistical values of June and December are compared;

- In order to observe how many rows of data in the two data sets, it is necessary to look at the statistics in the count part. It is observed that both tables do not have equal values and 183 rows of data are not included in the December analysis.

- While the average temperature was approximately 75 for the month of June, it was 71 for the month of December. Normally, when the temperature values in Table 3 for the month of December are taken into account and it should be noted that the lowest value observed in the table above is 56 degrees, 71 degrees is extremely high in terms of average and being a cold month.

- Looking at Table 2 and Table 4, it can be determined that the average temperature values of both months are very close to the median value.

- Considering the average, minimum, maximum temperature values and cartridge values in general; It is clear that there is not much difference between the temperatures. However, it can be stated that it still makes it more cold in December. However, according to the tables for the months of June and December, it can be estimated that the weather is not very cold, even if it is necessary to reach a general opinion.







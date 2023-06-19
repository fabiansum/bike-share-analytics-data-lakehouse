# Building An Azure Data Lake for Bike Share Data Analytics

## Project Overview
Divvy is a bike sharing program in Chicago, Illinois USA that allows riders to purchase a pass at a kiosk or use a mobile application to unlock a bike at stations around the city and use the bike for a specified amount of time. The bikes can be returned to the same station or to another station. The City of Chicago makes the anonymized bike trip data publicly available for projects like this where we can analyze the data.

Since the data from Divvy are anonymous, fake rider and account profiles along with fake payment data to go along with the data from Divvy have been generated. The dataset looks like this:

![Relational ERD for the Divvy Bikeshare Dataset (with fake data tables)](images/dend-project-erd.jpeg)

### Business Requirements
1. Analyze the duration of each ride:
    - Based on date and time factors such as day of the week and time of day
    - Based on the starting and/or ending station
    - Based on the rider's age at the time of the ride
    - Based on whether the rider is a member or casual rider
2. Analyze the cost:
    - Per month, quarter, and year
    - Per member, based on the rider's age at account start
3. Analyze the cost per member:
    - Based on the number of rides the rider averages per month
    - Based on the number of minutes the rider spends on a bike per month

### Technology Stack
- Azure Databricks

## Solution Architecture


## STAR Schema Design - Gold layer
The STAR schema consists of two fact tables (Fact Trip and Fact Payment) and three dimension tables (Dim Calendar, Dim Rider, Dim Station). 
![Star Schema](images/star_schema_fabian.png)
[Star Schema &mdash; PDF](https://github.com/fabiansum/bike-share-analytics-data-lakehouse/blob/main/pdf/star_schema_fabian.pdf)
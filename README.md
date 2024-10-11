# Car-Sales-Analysis-Report

## INTRODUCTION 

Analysing the Car Sales Dataset, which includes information on various automobile models, manufacturers, and other features in relation to sales and pricing, is the project's goal. The job is to examine the information and respond to the following queries:  
- Which Manufacturer has the highest and lowest average sales volume?
- How are the prices of cars distributed?
- Is there a correlation in the numerical variables of the dataset?
- Which is the most popular car brands?
- What is the top 3 fuel-efficient cars with an engine size above 2.5 litres? 

The main goal of this investigation is to demonstrate if car production, cost, and efficiency have increased significantly over time. Python would be used for the study in order to produce charts and carry out statistical analysis in a way that is simple to comprehend. 

## DATA SOURCING 
As part of the  assessment for the PSP Data Analytics coursewhich is taught by Mr. Joseph Elijah, the data was obtained from a Google Drive link and published to a WhatsApp group. The assessment question file and the car sales csv file were both in the folder.  

## DATA PREPARATION 

In preparing Data the required Python libraries will be imported to set up the Python environment before we begin analysis.  Matplotlib and Seaborn are used to visualise data, Numpy is imported to work with numbers and integers, Pandas, Series, and Dataframes. As seen in the figure below, we then read in the data in csv format. 

## DATA EXPLORATION 

To explore the data;
- The number of columns and rows in the data are counted. The dataset consists of 157 rows and 16 columns.
- Using the "dtypes" function, we next determine the datatypes of each column in the automobile sales data. 

The "Launch_date" column is the only one that is categorised as an object rather than a datetime object. Otherwise, it is evident that all columns with string values are classed as "objects" and all columns with integers or decimals are classified as "float" data types. 

- The "isna()" function is used to search the dataset for missing values. The SUM function is used to count each of them for each variable. 

## DATA CLEANING AND MISSING VALUES 

Before beginning the study, the data had been thoroughly cleaned. 

- The missing values are now handled in the following manner after being checked for. Out of the year_resale_value columns, about 36 have null or missing data. First, the average of all the columns are calculated to deal with them, and then substitute those values for the null values.
- Then, any more  rows that have missing data are removed. 

### RENAMING COLUMNS 
- The leading underscore from the column name '_year_resale_value' is removed.
- The dataset is then examined  to look for duplicates, but none are found.  

## DESCRIPTIVE STATISTICS 

- Here, a descriptive statistic of the numerical columns to find the mean, median, mode and others. We use the describe() function with specifying all, because we need just the numerical columns.
  ![image](https://github.com/user-attachments/assets/9fd970d2-cd01-4222-a0c5-0a8d57e63ecb)

 
## EXPLORATORY DATA ANALYSIS 

**1. Which Manufacturer has the highest and lowest average sales volume?**

By combining the Manufacturers according to their mean Sales in thousands and then arranging them in either ascending or descending order, we may determine which is the highest and lowest. To determine the highest and lowest average sales volume, respectively, we may also utilise idmax() and idxmin() in instead of sorting. 

**2. Distribution of car prices in the dataset**

  In this case, we aggregate and chart the Manufacturer using the total price expressed in thousand. 

**3. Correlation matrix of numerical variables in the dataset**
 
 ![image](https://github.com/user-attachments/assets/1e82b4bd-9b3d-462e-9ea7-a5f5ea5fd676)

**4. Which is the most popular car brands?**

When we combine the Manufacturer with the highest sales in thousands, we can observe that Ford is the most popular car, especially the F-Series model.

**5. What is the top 3 fuel-efficient cars with an engine size above 2.5 litres?**
 
 ![image](https://github.com/user-attachments/assets/e1d57858-8927-4bb3-a2c3-b9fec7e8de5e)

## CONCLUSION AND SUGGESTIONS 
Analysis on this data has offered  insightful, fact-based responses to business enquiries. It is advised that a comprehensive study be performed on a sizable dataset. After then, PowerBI and other sophisticated analytics tools can be used for visualisations.



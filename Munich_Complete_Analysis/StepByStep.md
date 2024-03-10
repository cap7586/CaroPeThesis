# Step by Step guide
## 1°) Import the necesary libraries
## 2°) Import CSV files into variables
## 3°) Create dataframes with the data from the CSV files
## 4°) Make sure the format of all different data frames match
-> format of the "datum" column (yyyy.mm.dd) is different to the one of the other years "yyyy-mm-dd"
## 5°) Concatenate all data frames to integrate them into one
## 6°) Drop columns that are not needed
## 7°) Time Series Analysis
### A) Add the date as index in our dataframe
### B) Drop columns that are not needed -> all locations will be added together for now, and we will concider "Munich" as one location
### C) Summarize the data
### D) 


# Urban Cycling Dynamics: A Comprehensive Analysis of Bike Counts in Germany - Part 1
## Introduction to the Topic and Analysis of the first City: Munich
Cycling has become a key mode of transport in urban areas around the world, offering numerous benefits from reducing traffic congestion to promoting environmental sustainability and public health. As German cities adopt cycling as a key component of their transportation networks, understanding the dynamics of cycling becomes paramount for urban planners, policy makers, and transportation enthusiasts alike. As part of my Bachelor thesis, this research embarks on an in-depth analysis of bicycle counts in several cities in Germany, with the goal of uncovering patterns, trends, and insights into urban cycling behavior. In this effort, I begin our exploration with Munich, a city known for its robust cycling infrastructure, progressive policies, and vibrant cycling culture.
## 1°) Ask: Questions that I want to answer.
What are the trends in bicycle usage across different locations in Munich over the years?
Are there any notable patterns or anomalies in the daily bike count data for each location?
How do seasonal variations impact bicycle usage in Munich, and do they vary between locations?
Are there any significant changes in bike usage trends during the COVID-19 pandemic period?
Which locations demonstrate the highest and lowest average daily bike counts, and what factors might contribute to these differences?
Are there any correlations between weather conditions (such as temperature, precipitation, or sunshine hours) and bike usage patterns?
Do certain locations exhibit more consistent or stable bike usage trends compared to others?
What insights can be gained from comparing bike usage trends across different locations within Munich?
Are there any external factors, such as nearby construction or infrastructure changes, that may influence bike usage patterns at specific locations?
How do the observed trends align with expectations or assumptions about urban cycling dynamics in Munich?

## 2°)
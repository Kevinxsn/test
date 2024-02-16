---
title: Home
layout: home
---
# Project 4 Housing Price

---

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---


## Overview

Housing prices serve as a key indicator of a region's economic health. The fluctuation of housing prices over time offers insights into the region's development to a certain degree. In this project, you will explore notable trends in housing prices over the past decade, alongside their correlation with changes in environmental conditions such as precipitation and temperature. An exciting aspect of this project is the opportunity to select the datasets you find most compelling for the topic you chose. You will engage in data manipulation techniques such as concatenation and merging of DataFrames, skills that were introduced at the start of this course!

## Getting The Data
You can get the data from [`here`](https://github.com/Kevinxsn/test/tree/main/data). 
You can also download the data from this shared [`google drive folder`](https://drive.google.com/drive/folders/1ECKr_Vmvjymr5zoRfysYCR-w47eXPj3M?usp=sharing). 

The data about housing prices is provided by [`Zillow`](https://www.zillow.com/). The data about the weather is provided by [`United States Census Bureau`](https://www.census.gov/). 

## Data Introduction

### population.csv
This dataset provide the information of the population changes over the past few years in different counties. 

| Header | Description |
| --- | --- |
| **STATE** | Numbered starting from 1, in the order of the first letter of each state. |
| **COUNTY** | Numbered starting from 1, in the order of the first letter of each county in each state. |
| **STNAME** | Name of each state. |
| **CTYNAME** | Name of each county. |
| **POPESTIMATE XXXX** | Estimated population based on census in year XXXX. |
| **NPOPCHG XXXX** | Estimated population change based on census in year XXXX. |
| **BIRTHS XXXX** | Estimated number of births based on census in year XXXX. |
| **DEATHS XXXX** | Estimated number of deaths based on census in year XXXX. |
| **NATURALCHG XXXX** | Estimated number of deaths based on census in year XXXX. |
| **INTERNATIONALMIG XXXX** | Estimated number of international imigrant based on census in year XXXX. |
| **DOMESTICMIG XXXX** | Estimated number of domestic imigrant based on census in year XXXX. |
| **NETMIG XXXX** | Estimated number of net imigrant based on census in year XXXX. |
| **RBIRTH XXXX** | Estimated birth rate based on census in year XXXX. |
| **RDEATH XXXX** | Estimated death rate based on census in year XXXX. |
| **RNATURALCHG XXXX** | Estimated rate of natural population change based on census in year XXXX. |
| **RINTERNATIONALMIG XXXX** | Estimated rate of international imigrant change based on census in year XXXX. |
| **RDOMESTICMIG XXXX** | Estimated rate of demostic imigrant change based on census in year XXXX. |
| **RNETMIG XXXX** | Estimated rate of net inmigrant change based on census in year XXXX. |


### housing_price.csv
This dataset provide the information of the housing price changes over the past few years in different counties. 

| Header | Description |
| --- | --- |
| **RegionID** | ID of each county in the US. |
| **SizeRank** | Ranking of each county based on size. |
| **RegionName** | Name of each region. |
| **RegionType** | Type of each region, in this case, all of them are counties. |
| **StateName** | The name of state that this region belongs to. |
| **Metro** | The name of metro that this region belongs to. |
| **StateCodeFIPS** | County FIPS codes in the United States are usually (with a few exceptions) in the same sequence as alphabetized county names within a state. |



### perXXXX.csv
It's a dataset contains the precipitation for the year of XXXX. Feel free to only load the dataset file that useful for your project. 

| Header | Description |
| --- | --- |
| **Name** | Name of each county. |
| **State** | The name of state that this county belongs to. |
| **Value** | mean precipitation for this year in this county in inches. |
| **Rank** | Ranking of the precipitation of the this county among all of the counties in the US, from low to high. |
| **Anomaly (1901-2000 base period)** | The degree of abnormality observed over the past few years(based on 1901-2000). |
| **1901-2000 Mean** | The mean precipitation of this region from 1901-2000. |


### GDP.xlsx
Gross Domestic Product (GDP) is the total monetary value of all goods and services produced within a country's or region's borders in a specific time period, serving as a broad measure of its economic activity.

| Header | Description |
| --- | --- |
| **Region** | Name of each region(note; it countains moth of the state name and county name). |
| **GDP XXXX (thousand of dollars)** | GDP in this region, in the unit of thoudsnd of dollars. |
| **Rank Iin States XXXX (Overall)** | The ranking of GDP of the county within the state in the year XXXX, from high to low. |
| **Percent Change XXXX** | Percent of GDP change in the year of XXXX. |


### tempXXXX.csv
It's a dataset contains the temprature for the year of XXXX. Feel free to only load the dataset file that useful for your project. 

| Header | Description |
| --- | --- |
| **Name** | Name of each county. |
| **State** | The name of state that this county belongs to. |
| **Value** | mean temprature for this year in this county in  Fahrenheit. |
| **Rank** | Ranking of the temprature of the this county among all of the counties in the US, from low to high. |
| **Anomaly (1901-2000 base period)** | The degree of abnormality observed over the past few years(based on 1901-2000). |
| **1901-2000 Mean** | The mean temprature of this region from 1901-2000. |



## Sample Questions
1. How do changes in GDP correlate with housing price trends in different counties? 
2. Is there a correlation between average temperature or precipitation levels and housing prices in a region?
3. How does population growth in each county affect housing prices over time?
4. Are there any short-term fluctuations in housing prices that correlate with extreme weather events or sudden changes in economic conditions?
5. How has the affordability of housing (housing prices relative to GDP per capita or average incomes) changed over time in different counties?


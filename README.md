# DS606-Capstone

# Predicting Car Crash Severity and Frequency in Maryland

This project repository includes all of the code and analysis of predicting car crash severity and frequency by training a machine learning model to find the most relevant risk factors for different kinds of vehicle crashes in the State of Maryland.

- [Introduction](#introduction)
- [Methodology](#methodology)
- [Modeling Results and Discussions](#modelingresultsanddiscussions)
- [Limitations and Challenges](#limitationsandchallenges)

---
## Introduction

Traffic accidents pose a significant public safety concern, leading to numerous injuries and fatalities worldwide. According to WHO [1], every year the lives of approximately 1.19 million people are cut short because of a road traffic crash. Between 20 and 50 million more people suffer non-fatal injuries, with many incurring a disability. In the U.S., according to the National Highway Traffic Safety Administration (NHTSA), an estimated 20,190 and 19,515 people died in motor vehicle traffic crashes in 2022 and 2023 respectively in spite of the decline in traffic fatalities after Covid-19 pandemic. Traffic deaths are continuing to slowly come down—but that is still a long way to go to achieve the expected safety standard set at the core mission of the U.S. Department of Transportation. Maryland is dedicated to saving lives and preventing injuries and fatalities resulting from motor vehicle crashes. Despite new advances, in-vehicle technology, such as backup cameras, adaptive headlights, and advanced collision warning systems, motor vehicle crashes still happen. 

One of the major missions of the transportation profession is to prevent accidents and to reduce risk of severe accidents; identifying the key factors affecting crash severity and their effects is important for policy and traffic operations to achieve that mission. Therefore, numerous studies have investigated the contributing factors using various types of models. Predictive safety analysis is one important step towards implementing proactive approaches to improve traffic safety. This marks a shift from primarily focusing in a reactive way on locations where crashes have occurred to more proactive and systemic approaches that identify and treat locations that have high risk for crashes in the future. 
For this, machine learning techniques have recently been introduced as an alternative to traditional data analysis methods to investigate factors associated with injury severity. It enables the extraction of important knowledge from significant amounts of complicated and heterogeneous data. The most widely used machine learning techniques are decision trees (DT), Bayesian networks, classification and regression trees, extreme gradient boosting, and random forest (RF).

This project is designed to reduce the number of crashes across Maryland by training a machine learning model to find the most relevant risk factors for different kinds of vehicle crashes (fatal, injury, or property damage). Different risk factors include location, speed limit, driver status, road status, weather, etc. Crash severity prediction models enable different agencies to predict the severity of a reported crash with unknown severity or the severity of crashes that may be expected to occur sometime in the future. The model was accompanied by maps visualizing roads and areas that are highly concentrated with crashes. Depending on which features the model believes to be the most important, state agencies could concentrate more resources on addressing those issues specifically. As a result, the Maryland Highway Safety Office focuses on areas that address behaviors resulting in crashes including speed and aggressive driving, distracted driving, impaired driving, motorcyclists, pedestrian and bicyclist and car seats and booster seats.


## Goals

The purpose of this project is to predict car crash severity and frequency by training a machine learning model to find the most relevant risk factors for different kinds of vehicle crashes (fatal, injury, or property damage) and gain useful insight about vehicle crashes within the state of Maryland.

<a id="methodology"></a>

## Methodology

In this section, the dataset used in our study is presented along with the data preprocessing activities.

### Data Preparation

This project used data obtained from the  [**Maryland Crash Database**](https://mdsp.maryland.gov/Pages/Dashboards/CrashDataDownload.aspx). Available data is compiled from Police crash reports approved and submitted to the Maryland Department of State Police (MDSP) via the Automated Crash Reporting System (ACRS). Crash locations reflect the approximate locations of the incident based on longitudinal and latitudinal information provided by the officer  through ACRS. The dataset provides general information about each incident tracked with a report number and includes driver, nonmotorist, passenger, vehicle and collision circumstances occurring on all county and local roadways, and state and interstate highways within the State of Maryland, as collected via the Automated Crash Reporting System (ACRS) of the Maryland State Police. The dataset is updated daily, and the version used for this project contains data from January 2020 to December 2023. In a given year there are about 100,000 reported incidents. They also provide a shapefile of main public roads in the whole state.

The information from this dataset used for the model and visualization include among others, crash report type, crash date/time, route types/name, collusion type, weather and surface condition, driver substance abuse. Using python and R packages and libraries, the data will be read and basic data tidying was performed to drop na values, unnecessary columns and any incomplete records and further the data has been transformed. Using ggplot visualization packages, the data has been further explored, visualized and mapping will be performed to identify crashes within each road in the State.

### Data Preprocessing

Data preprocessing is an integral step in machine learning as the quality of data and the useful information that can be derived from it directly affects the ability of our model to learn; therefore, it is extremely important that we preprocess our data before feeding it into our model.
Analyzing motor vehicle crash data using machine learning involves several key steps. Here's a more detailed breakdown of the process. This dataset was cleaned up, transformed, and pre-processed to build and train the predictive models. It is because some of the data columns contain redundant data, or are uncorrelated to the prediction target, or consist of missing values. 

![Methodology Final](https://github.com/dennisp12umbc/DS606-Capstone/assets/90659371/6b44cccc-8a1e-4bb0-8b98-453d99e4271f)





### Exploratory Data Analysis (EDA)

<a id="modelingresultsanddiscussions"></a>

## Modeling Results and Discussions

<a id="limitationsandchallenges"></a>

## Limitations and Challenges


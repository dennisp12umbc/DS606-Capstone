# DS606-Capstone

# Predicting Car Crash Severity and Frequency in Maryland

This project repository includes all of the code and analysis of predicting car crash severity and frequency by training a machine learning model to find the most relevant risk factors for different kinds of vehicle crashes in the State of Maryland.

- [Introduction](#introduction)
- [Methodology](#methodology)
- [Modeling Results and Discussions](#modelingresultsanddiscussions)
- [Limitations and Challenges](#limitationsandchallenges)

---
## Introduction

Traffic accidents pose a significant public safety concern, leading to numerous injuries and fatalities worldwide. According to WHO, every year the lives of approximately 1.19 million people are cut short because of a road traffic crash. Between 20 and 50 million more people suffer non-fatal injuries, with many incurring a disability. In the U.S., according to the National Highway Traffic Safety Administration (NHTSA), an estimated 20,190 and 19,515 people died in motor vehicle traffic crashes in 2022 and 2023 respectively in spite of the decline in traffic fatalities after Covid-19 pandemic. Traffic deaths are continuing to slowly come down—but that is still a long way to go to achieve the expected safety standard set at the core mission of the U.S. Department of Transportation. Maryland has about 500 fatal crashes and several thousand injury crashes per year. Maryland is dedicated to saving lives and preventing injuries and fatalities resulting from motor vehicle crashes. The Maryland Highway Safety Office uses a data-driven approach to try and minimize the number of fatal crashes down to zero. Despite new advances in car safety technology like backup cameras, adaptive headlights, and advanced collision warning systems, motor vehicle crashes still happen at high rates.

Policymakers want to reduce the number and severity of all accidents, and to do that they need to know what policy to push. A data-driven approach like how the MD Highway Safety Office does is especially important because it can show off the most important factors related to the cause of dangerous crashes. Without it, they would be primarily making educated guesses at what the real problems are. This could be misleading because there could be a factor that seems like it could be especially important, but in reality is not. The opposite can also be true, where a factor that was not known to be particularly important is actually the root cause of many crashes. Machine learning models like logistic regression, decision tree, and random forest are used in combination with traditional data analysis to better predict when and how car crashes will occur. Policymakers in the past have been more reactive in their response to growing numbers of crashes, but with this kind of predictive analytics, they can be more proactive and fight against dangerous factors ahead of time. Several studies have undergone this line of analysis in other locations like Chicago and Texas as well.

This project is designed to reduce the number of crashes across Maryland by training a machine learning model to find the most relevant risk factors for different kinds of vehicle crashes (fatal, injury, or property damage). Different risk factors include location, speed limit, driver status, road status, weather, etc. Crash severity prediction models enable different agencies to predict the severity of a reported crash with unknown severity or the severity of crashes that may be expected to occur sometime in the future. The model was accompanied by maps visualizing roads and areas that are highly concentrated with crashes. Depending on which features the model believes to be the most important, state agencies could concentrate more resources on addressing those issues specifically.

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

![Methodology Workflow](https://github.com/dennisp12umbc/DS606-Capstone/assets/90659371/c6d6a9d8-2bf5-494b-9ef7-b1b66c7d007c)






### Exploratory Data Analysis (EDA)

<a id="modelingresultsanddiscussions"></a>

## Modeling Results and Discussions

<a id="limitationsandchallenges"></a>

## Limitations and Challenges


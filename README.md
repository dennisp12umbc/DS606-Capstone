# DS606-Capstone

# Predicting Car Crash Severity and Frequency in Maryland

This project repository includes all of the code and analysis of predicting car crash severity and frequency by training a machine learning model to find the most relevant risk factors for different kinds of vehicle crashes in the State of Maryland.

- [Background](#background)
- [Literature review](#literaturereview)
- [Methodology](#methodology)
- [Data Preparation](#datapreparation)
- [Modeling Results and Discussions](#modelingresultsanddiscussions)
- [Limitations and Challenges](#limitationsandchallenges)

---
## Background

Motor vehicle crashes are a public health concern both in the United States and abroad. Traffic crash analysis can be used to analyze crash data and identify streets and intersections where concentrations of serious and fatal crashes occur. It is an integral component of transportation engineering and traffic safety advocacy. Such analysis provides valuable insights that inform decision-making, guide interventions, and contribute to the overall goal of creating safer and more efficient transportation systems.

Accurate crash analysis helps insurers make informed decisions and ensures fair compensation for policyholders involved in accidents. Understanding the dynamics of crashes helps emergency responders better prepare for and respond to accidents. This includes developing effective rescue techniques, optimizing ambulance services, and improving hospital trauma care. In addition, crash data is used to identify high-risk areas on road networks. This information is crucial for planning and implementing changes to road infrastructure, such as installing traffic signals, improving road signage, and implementing traffic safety measures to limit vehicle collisions. 

This project is designed to reduce the number of crashes across Maryland by training a machine learning model to find the most relevant risk factors for different kinds of vehicle crashes (fatal, injury, or property damage). Different risk factors include location, speed limit, driver status, road status, weather, etc. Crash severity prediction models enable different agencies to predict the severity of a reported crash with unknown severity or the severity of crashes that may be expected to occur sometime in the future. The model will be accompanied by some maps visualizing roads and areas that are highly concentrated with crashes.

Depending on which features the model believes to be the most important, state agencies could concentrate more resources on addressing those issues specifically. For example, if the speed limit does not appear to be significant while drunk driving does, then perhaps agencies would reduce the number of state troopers at speed traps in favor of police checkpoints.

## Goals

The purpose of this project is to predict car crash severity and frequency by training a machine learning model to find the most relevant risk factors for different kinds of vehicle crashes (fatal, injury, or property damage) and gain useful insight about vehicle crashes within the state of Maryland.

<a id="methodology"></a>

## Methodology

### Data Collection

This project used data obtained from the  [**Maryland Crash Database**](https://mdsp.maryland.gov/Pages/Dashboards/CrashDataDownload.aspx). Available data is compiled from Police crash reports approved and submitted to the Maryland Department of State Police (MDSP) via the Automated Crash Reporting System (ACRS). Crash locations reflect the approximate locations of the incident based on longitudinal and latitudinal information provided by the officer  through ACRS. The dataset provides general information about each incident tracked with a report number and includes driver, nonmotorist, passenger, vehicle and collision circumstances occurring on all county and local roadways, and state and interstate highways within the State of Maryland, as collected via the Automated Crash Reporting System (ACRS) of the Maryland State Police. The dataset is updated daily, and the version used for this project contains data from January 2020 to December 2023. In a given year there are about 100,000 reported incidents. They also provide a shapefile of main public roads in the whole state.

The information from this dataset used for the model and visualization include among others, crash report type, crash date/time, route types/name, collusion type, weather and surface condition, driver substance abuse. Using python and R packages and libraries, the data will be read and basic data tidying was performed to drop na values, unnecessary columns and any incomplete records and further the data has been transformed. Using ggplot visualization packages, the data has been further explored, visualized and mapping will be performed to identify crashes within each road in the State.

### Data Preporocessing

Data preprocessing is an integral step in machine learning as the quality of data and the useful information that can be derived from it directly affects the ability of our model to learn; therefore, it is extremely important that we preprocess our data before feeding it into our model.
Analyzing motor vehicle crash data using machine learning involves several key steps. Here's a more detailed breakdown of the process. This dataset was cleaned up, transformed, and pre-processed to build and train the predictive models. It is because some of the data columns contain redundant data, or are uncorrelated to the prediction target, or consist of missing values. 
![Methodology_Edited](https://github.com/dennisp12umbc/DS606-Capstone/assets/90659371/6f3adc1f-258e-4fe9-b382-9140ddc7d06a)


### Exploratory Data Analysis (EDA)

<a id="modelingresultsanddiscussions"></a>

## Modeling Results and Discussions

<a id="limitationsandchallenges"></a>

## Limitations and Challenges


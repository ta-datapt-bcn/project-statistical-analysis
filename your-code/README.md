<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Statistical Analysis Project
*Daniel Eiroa*

*Data Part-Time | Barcelona | May 2019*

## Content
- [Project Description](#project-description)
- [Hypotheses / Questions](#hypotheses-/-questions)
- [Dataset](#dataset)
- [Cleaning](#cleaning)
- [Analysis](#analysis)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Conclusion](#conclusion)
- [Future Work](#future-work)
- [Workflow](#workflow)
- [Organization](#organization)
- [Links](#links)

<a name="project-description"></a>

## Project Description
The objective of the project is to integrate data analysis and statistical analysis tools and methods learnt throughout this module.
I've chosen a dataset that contains every flight from or to a United States airport during the year 2015. 

<a name="hypotheses-/-questions"></a>

## Hypotheses / Questions
The specifics about questions and hypotheses are detailed in the notebook.
In general terms, I wanted to demonstrate how the volume of operations of the airports and airlines influence delays. Also, some analysis on how the day of the week may influence delays was carried out.

<a name="dataset"></a>

## Dataset
I chose a dataset from Kaggle including all the flights from/to the US during the year 2015. [link](https://www.kaggle.com/usdot/flight-delays#flights.csv)
It is a pretty large dataset (more than 6 million rows) that I had to filter from the beginning for performance issues.
The dataset contains the following 31 columns.
**Column Explanations**
* YEAR: Year of the Flight Trip
* MONTH: Month of the Flight Trip
* DAY: Day of the Flight Trip
* DAY_OF_WEEK: Day of week of the Flight Trip
* AIRLINE: Airline Identifier
* FLIGHT_NUMBER: Flight Identifier
* TAIL_NUMBER: Aircraft Identifier
* ORIGIN_AIRPORT: Starting Airport
* DESTINATION_AIRPORT: Destination Airport
* SCHEDULED_DEPARTURE: Planned Departure Time (as integer: first two digits hour, other two digits minutes)
* DEPARTURE_TIME: Actual Departure Time
* DEPARTURE_DELAY: Total Delay on Departure (in minutes). If + Delayed, if - Before.
* TAXI_OUT: The time duration elapsed between departure from the origin airport gate and wheels off
* WHEELS_OFF: The time point that the aircraft's wheels leave the ground
* SCHEDULED_TIME: Planned time amount needed for the flight trip
* ELAPSED_TIME: AIR_TIME+TAXI_IN+TAXI_OUT
* AIR_TIME: The time duration between wheels_off and wheels_on time
* DISTANCE: Distance between two airports
* WHEELS_ON: The time point that the aircraft's wheels touch on the ground
* TAXI_IN: The time duration elapsed between wheels-on and gate arrival at the destination airport
* SCHEDULED_ARRIVAL: Planned arrival time
* ARRIVAL_TIME: WHEELS_ON+TAXI_IN
* ARRIVAL_DELAY: ARRIVAL_TIME-SCHEDULED_ARRIVAL. If + Delayed, if - Before.
* DIVERTED: Aircraft landed on airport that out of schedule
* CANCELLED: Flight Cancelled (1 = cancelled)
* CANCELLATION_REASON: Reason for Cancellation of flight: A - Airline/Carrier; B - Weather; C - National Air System; D - Security
* AIR_SYSTEM_DELAY: Delay caused by air system
* SECURITY_DELAY: Delay caused by security
* AIRLINE_DELAY: Delay caused by the airline
* LATE_AIRCRAFT_DELAY: Delay caused by aircraft
* WEATHER_DELAY: Delay caused by weather

<a name="cleaning"></a>

## Cleaning
* Creating a subset only with the delayed flights to work with a lighter dataset.
* Overview of the dataset.
* Filtering out the columns and rows with null values.
* Dropping columns that were complete but weren't useful for the analysis.
* Cleaning outliers using the IQR method.
* Plotting distributions and correlations using heatmap.
* Changing Year, Month, Day columns to DateTime and combining them in a unique column.

<a name="analysis"></a>

## Analysis
* Descriptive statistics for departure and arrival delays by airport and airlines, with confidence intervals.
* Proportion of long delay flights among all flights, with confidence intervals.
* Proportion of long delay flights among all the flights of #1 company in terms of number of flights, with confidence intervals.
* Proportion of long delay ORIGIN flights in the #1 Airport in terms of number of total departures, with confidence intervals.
* Proportion of long delay DESTINATION flights in the #1 Airport in terms of number of total arrivals, with confidence intervals.

* Hypothesis testing: Is there a significant correlation between mean departure and arrival delay for those flights delayed longer than 2h in the TOP30 US airports?
* Hypothesis testing: Are arrival delays on weekends (Fri-Sat-Sun) significantly different from those on weekdays (Mon-Tue-Wed-Thu) for flights delayed in the TOP30 US airports?
* Hypothesis testing: Are there differences between variances on the arrival delay for the TOP5 airlines?
* Hypothesis testing: Are there differences between variances on the arrival delay for the TOP30 airports?
* Hypothesis testing: Is the difference of mean arrival delay significant between #1 and #2 airlines for those flights delayed longer than 2h?
* Hypothesis testing: Is there a significant difference on the porportion of long delay flight among all flights between the #1 airport and the rest of airports?

<a name="conclusion"></a>

## Conclusion
* As detailed in the notebook, some of the hypotheses were rejected but others could not.
* The narrowness of some of some confidence intervals surprised me. I suppose it is due to the size of the sample.


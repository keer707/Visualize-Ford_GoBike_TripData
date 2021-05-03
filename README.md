# Ford GoBike TripData Exploration

## Dataset

The dataset includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area of the ford gobike for the year 2018.

For this analysis, I have downloaded 2018 datasets, which are 12 CSVs for each month.

**Brief description about the data :**
- Trip Duration (seconds)
- Start Time and Date
- End Time and Date
- Start Station ID
- Start Station Name
- Start Station Latitude
- Start Station Longitude
- End Station ID
- End Station Name
- End Station Latitude
- End Station Longitude
- Bike ID
- User Type (“Subscriber” = Member or “Customer” = Casual)
- Member Year of Birth
- Member Gender
- Bike Share for all Trip

**DataSource:** [Ford GoBike](https://s3.amazonaws.com/fordgobike-data/index.html)

Also, you can get the merged data [here](https://www.kaggle.com/keerthanamanoharan/ford-gobike-tripdata-2018)


## Summary of Findings

In the exploration, I found that there are many factors of users and trips influencing the trip frequency and trip duration.

**Factors affecting Trip Frequency,**
> **User Features** : Subscribers have contributed in more frequent trips than Customers, among which Male has the highest number of trip counts compared to other gender types. Users aged between 25-50 has the frequent and low duration trips.

> **Trip Features** : The hour of the day and Day of the week has an impact on trip frequency, where **Weekdays** being the highest trip holders with peak hours of **8am-9am** and **5pm-6pm**

> **User & Trip** : In **Busy hours (8am & 5pm)**, frequency of **Subscriber** trips is higher than **Customer** trips during morning, while in the evening frequency of **Customer** trips is almost equal to **Subscriber** trips in **Week Days**. The frequency of trips in **Week ends** is higher for **Customer** rather than **Subscriber** during day time (10am-5pm)

**Factors affecting Trip Duration,**
> **User Features** : Customers have contributed in more high duration trips than Subscribers, among which users without personal information registered has the highest trip duration, followed by Female compared to other gender types. Users aged above 100 has the high duration trips.

> **Trip Features** : The hour of the day and Day of the week has an impact on trip duration, where **Weekends** being the high duration trips holders with peak hours of **1am-3am** and **9am-5pm**

> **User & Trip** : Early morning around **1am-4am**, user aged **60** goes for **high duration trips**. While, few elder users aged above **100** go for higher duration trips during **day time (5am-5pm)**. For both Customer and Subscriber, weekends have the higher trip duration, among which Customer has the highest.

The Busiest Route is from **San Francisco Ferry Building (Harry Bridges Plaza)** (ID:15) to **The Embarcadero at Sansome St** (ID:6) with trip count of **7585**

## Key Insights for Presentation

For the presentation, I focus on the influence of the **User & Trip** features on **Trip frequency & duration**. I start by introducing the distribution of trip duration (log scale) with respect to trip frequency. Then, I continue by plotting the distributions of trip features, Hour of the Day and Day of the Week. And also user features, gender and user type.

Following, I plot the relationship between trip duration, trip frequency and Age using heat map. Then, I continue plotting the hourly frequency for each day of the week for users having the highest trip counts in the previous graph.

Afterwards, I planned to plot the average trip duration for gender and user type. Then, I plot the relationship between day of the week and user type associated with trip duration. I plot the User's age contribution in trip duration for each hour.

At last, I plot the busiest 20 routes.


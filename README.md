# (FordGoBike Data Exploration)
## by (Oluwafunmilayo Chinonye Samuel)


## Dataset

The data consists of information on a bike sharing system in the greater San Francisco Bay area for roughly 183, 000 rides for February, 2019. Some preliminary wrangling was done before exploration including some feature engineering, dropping null values and unneeded columns, and changing wrong data types. A deepcopy was created for the wrangling process to avoid tampering with the original dataset provided. The final dataset contains 174952 bike share rides with 14 columns. Below is a brief description of each column variable:

start_station_id - 329 unique ids
start_station_name - 329 unique names
end_station_id - 329 unique ids
end_station_name - 329 unique names
bike_id - 4607 unique ids
user_type - Customer or Subscriber
gender - Male, Female or Other
bike_share_for_all_trip - was the bike share used for the entire trip? Yes or No
distance - distance between start and end stations
duration_hr - trip duration in hours
age - age of the member
day_name - Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday
time - morning, afternoon, early evening, late evening, night
day_week - Weekday or Weekend
Majority of the variables are categorical, and there are three numeric variables (distance, duration_hr, and age).


## Summary of Findings

The exploration focused on finding the differences between user types and possible determinants that influenced user type. 90% of the users were subscribers and 9% were customers. Trip duration, distance, and bike share for all trip were significant determinants of the differences in user type. Majority of the trips were taken on Weekdays compared to weekends, and the day with the highest trips were Thursdays. Customers had a higher trip duration, and distance compared with subscribers. Furthermore, only subscribers used the bike share for entire trips. It was ascertained that the majority of the subscribers who used the bike share for the entire trip travelled for smaller durations and distances, with some travelling for longer hours, and covering more distances than others. 

There were also interesting interactions between the other variables, and there were also some interesting insights uncovered during the multivariate exploration for variables which were not initially identified as significant determinants of differences in user type. Trip duration was moderately positively correlated with distance, and a 1km increase in distance caused a 0.07hr (4.2mins) increase in trip duration. This was attributed to the fact that distance accounts for 26% of the changes in trip duration, and is thus a significant part of the trip duration. It was quite surprising that there was no correlation between the age of the bike sharers and the trip duration because research often confirms this fact. However, the fact that the median age across gender and user type indicated that the bike sharers belonged to the working class was concluded as the possible explanation for this finding. Finally, the exploration revealed that females biked longer distances compared with the other gender types, and most customers used the bike share for biking longer hours during the weekends, and in the afternoons. 

## Key Insights for Presentation

Although the exploration revealed numerous insights, I will focus the presentation on the effects of trip duration, distance, and bike share for all trip on user type. I will begin with an introduction of the individual distribution for the four variables, focusing on the final distribution after the intermediary cleaning processes. Then, I will proceed with the individual and combined effects of the significant determinats on user type. I will also include the insight on the strong relationship between trip duration and distance, as this provided a very key statistical insight. 

Finally, I will add some intersting additional insights from the interactions for combined variables like that of the gender, time category, and day category. 
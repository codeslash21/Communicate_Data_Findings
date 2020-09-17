# Ford GoBike System Data Exploration
## by Soumyadip Guha

</br>

<div style="font-size:18px">
    
### About Dataset    

   Here we analyze <a href="https://en.wikipedia.org/wiki/Bay_Wheels">Bay Wheels</a>(previously known as Ford GoBike) System data. Bay Wheel is a regional public bicycle sharing system in the San Francisco Bay Area, California. Bay Wheels is the first regional and large-scale bicycle sharing system deployed in California. The dataset used for this exploratory analysis consists of monthly trip data from January 2019 to December 2019 covering the greater San Francisco Bay area. The dataset basically is the trip records under Bay Wheel. The dataset can be found <a href="https://www.lyft.com/bikes/bay-wheels/system-data">here</a>.

## Dataset Overview

<div style="font-size:18px">

Here we take trip records of the Year 2019. Our target is to explore the trends and find some interesting facts about the dataset. Primarily this dataset records 2.5M individual trips and every trip has 15 features. We can divide these features into three groups -
- bike_id, user_type, bike_share_for_all_trip [User related data]
- start_station_id, start_station_name, start_station_latitude, start_station_longitude, end_station_id, end_station_name, end_station_latitude, end_station_longitude [Stations related information]
- rental_access_method, start_time, duration_sec, end_time [trip related data]

We create some new column for ease of exploration and remove the columns those will not be used in this analysis. Finally our dataset consists of these columns - 'bike_id', 'end_station_name', 'end_time', 'rental_access_method',
       'start_station_name', 'start_time', 'user_type', 'duration_minute',
       'start_date', 'start_month', 'start_month_day', 'start_weekday',
       'start_hour', 'start_month_num', 'season'

</br>


## Summary of Findings

<div style="font-size:18px">
    
   In the exploration, I found that teo diffrent types of user present different behaviour in rides. I found that subscribers share around 80.6% and customers share around 19.4% in bike rides. Though customers are more likely to have long trips with average trip duration 22.55 minutes. Average trip duration for customers is around 11 minutes. Average trip duration over the week of customers is always greater than average trip durations of subscribers. On weekends though numbers of rides are less, average trip durations is more than average trip durations on working days. Basically there is no particular trends of rides over the year, there is ups and downs of trends through out the year. Though we found 'December' month has less number of rides and 'July' has highest number of rides. Over the week we found least numbers of rides on Sunday and highest numbers of rides on Tuesday. Lowest trip duration is 1 minute and longest trip duration is around 1437 minutes.
   
   Besides these main variables I explored the relationships between the rides and season, and found Spring is more comfortable for riders to ride with highest numbers of rides and Winter is less prefarable to ride. Though average trip duration in Summer is greater than average trip duration in other season.

</br>

## Key Insights for Presentation

<div style="font-size:18px">
    
  For presentation I focused on first distribution of rides over the month, season, week and hour. This is important to see the trends for improving business policies. Then I focused on different behaviours of different user types with these variables to get nice visualization of important factors.
  
  - **Rides trends over the year:** 
    - There is no particular trends that rides follows. Though in Winter we see less rides and in 'July' we see highest number of rides.
    - For cutomers there is an upward trends from 'May' to 'December', so we can say that this rides services being popular among the customers.
   
  - **Rides trends over season:**
    - We see higher number of rides in Spring and less rides in Winter, means Spring is more comfortable for riders to ride.
    - Though average trip duration in Summer is more.
   
  - **Rides trends over week:**
   - During weekends we see less number of rides.
   - On Tuesday we see highest number of rides.
   - Average trip duration of customers is always grater than that of subscribers over the week.
   
  - **Rides trends over hours:**
   - We have two rush hours 8A.M. and 5P.M.

</br>

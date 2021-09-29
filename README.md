# bikesharing
Module 14 - Tableau

## Project Overview

Support decision-making processes about a bike-sharing program in Des Moines. To solidify the proposal, one of the key stakeholders would like to see a bike trip analysis that:
- Show the length of time that bikes are checked out for all riders and genders
- Show the number of bike trips for all riders and genders for each hour of each day of the week
- Show the number of bike trips for each type of user and gender for each day of the week


Deliverable 1
- [x] 1. The data in the "tripduration" column is converted to a datetime datatype and has the correct time format
- [x] 2. The DataFrame is exported as a new file without the index column

[Jupyter Notebook file](https://github.com/GabrielaTuma/bikesharing/blob/7fed2962046b921c5f47bb515c9639a26fd7b630/NYC_Citibike_Challenge.ipynb) 

Deliverable 2
- [x] 1. There is a line graph displaying the number of bikes checked out by duration for all users, and the graph can be filtered by the hour
- [x] 2. There is a line graph displaying the number of bikes that are checked out by duration for each gender by the hour, and the graph can be filtered by the hour and gender
- [x] 3. A heatmap is created showing the number of bike trips for each hour of each day of the week
- [x] 4. A heatmap is created showing the number of bike trips by gender for each hour of each day of the week, and the heatmap can be filtered by gender
- [x] 5. A heatmap is created showing the number of bike trips for each type of user and gender for each day of the week, and you can only filter by user and gender


[Images folder](https://github.com/GabrielaTuma/bikesharing/tree/main/Images%20)


Deliverable 3
Structure, organization, and formatting:
- [x] 1. There is a title, and there are multiple sections
- [x] 2. Each section has a heading and subheading
- [x] 3. Links to images are working and displayed correctly
Written analysis:
- [x] 4. The purpose of the analysis is well defined
- [x] 5. There are at least seven visualizations for the NYC CitiBike analysis
- [x] 6. There is a description of the results for each visualization
- [x] 7. There is a high-level summary of the results and two additional visualizations are suggested for future analysis

[Tableau Story link](https://public.tableau.com/app/profile/gabriela.tuma/viz/Challenge14_16328427047360/Challenge14-Story)



## Resources 

- Software: Python 3.7.6, Visual Studio Code 1.58.1, Jupyter Notebook 6.3.0
- Tableau Desktop - Public Edition - version 2021.3.0
 
 
## Outcomes 
  
This analysis was done based on files from [CitiBike website](https://s3.amazonaws.com/tripdata/index.html), more specifically the data from August 2019.  

Out of the many outcomes possible, we started the analysis finding the amount of trips by hour of the day. Knowing the peak hours is very important to understand the business and plan for the future demand, this information is crucial to determine the amount of bikes and equipment available per station for example.  

<p align="center">
<kbd>
  <img src="https://github.com/GabrielaTuma/bikesharing/blob/7fed2962046b921c5f47bb515c9639a26fd7b630/Images%20/August%20Peak%20Hours.png">
</kbd>  &nbsp;
</p>

The August Peak Hours graph shows that the busiest hours are 7a.m. to 10a.m. and 4p.m. to 7p.m. Taking into account that the conventional workday remains pretty strong and the majority of people are at work from 9 a.m. to 5 p.m. it makes sense to assume that most of the business comes from rides right before or right after work. But is this applicable on the weekends? 


<p align="center">
<kbd>
  <img src="https://github.com/GabrielaTuma/bikesharing/blob/7fed2962046b921c5f47bb515c9639a26fd7b630/Images%20/Trips%20by%20Weekday%20per%20Hour.png">
</kbd>  &nbsp;
</p>

This heatmap can seem confusing at first but is very informative and can be useful to make strategic decisions such as maintenance hours and demand forecasting. 

The August Peak Hours graph done previously shows similar information, but the heatmap on the other hand brings another important variable: the day of the week. The different patterns created by weekends and weekdays emphasize the importance of looking at the data from more than one perspective. On the weekends the business is more steady throughout the day and the peak hours are around lunch time. Also, we can see that Wednesdays are visibly slower than any other day. 



<p align="center">
<kbd>
  <img src="https://github.com/GabrielaTuma/bikesharing/blob/7fed2962046b921c5f47bb515c9639a26fd7b630/Images%20/Trips%20by%20Gender%20(Weekday%20per%20Hour).png">
</kbd>  &nbsp;
</p>


Analyzing the Trips by Gender we notice a similar pattern for males and females, even though the colour intensity is visibly different. Which means that regardless of the the gender, customers have similar biking habits when it comes to day of the week and time, but males are still the majority in number of rides. 



<p align="center">
<kbd>
  <img src="https://github.com/GabrielaTuma/bikesharing/blob/7fed2962046b921c5f47bb515c9639a26fd7b630/Images%20/Gender%20Breakdown.png">
</kbd>  &nbsp;
</p>


Another relevant information we can take from CitiBike is that most of the customers are male, adding up to more than 70% compared to females. 

The gender doesn't seem to affect biking habits, but what about the user type? CitiBike allows customers to have a subscription and we should investigate if different users have similar habits. 




<p align="center">
<kbd>
  <img src="https://github.com/GabrielaTuma/bikesharing/blob/7fed2962046b921c5f47bb515c9639a26fd7b630/Images%20/User%20Trips%20by%20Gender%20by%20Weekday.png">
</kbd>  &nbsp;
</p>


By looking at the heatmap by user type we can say that customers without a subscription tend to use the services on the weekends while subscribers tend to use it during the week, probably to go to work given the peak hours. The gender once again seems irrelevant to the pattern. 

-------

<p align="center">
<kbd>
  <img src="https://github.com/GabrielaTuma/bikesharing/blob/7fed2962046b921c5f47bb515c9639a26fd7b630/Images%20/Checkout%20Times%20for%20Users%20.png">
</kbd>  &nbsp;
</p>




The Checkout Times graph makes it clear that the majority of trips are not longer than 20 minutes. 


<p align="center">
<kbd>
  <img src="https://github.com/GabrielaTuma/bikesharing/blob/7fed2962046b921c5f47bb515c9639a26fd7b630/Images%20/Checkout%20Times%20by%20Gender%20.png">
</kbd>  &nbsp;
</p>


Males and females show similar patterns when it comes to trip duration, most of the rides take around 10 minutes, regardless of the gender. 



## Summary 



Calculating the amount of resources necessary to build a profitable bike sharing company is one of the most important steps of the business plan. 


Given the data available we were able to plot a Bike Utilization Graph, for example. 


<p align="center">
<kbd>
  <img src="https://github.com/GabrielaTuma/bikesharing/blob/7fed2962046b921c5f47bb515c9639a26fd7b630/Images%20/Bike%20Utilization.png">
</kbd>  &nbsp;
</p>


CitiBike database provide us with trip duration, stations IDs, locations, bike IDs, birth year, gender, among others. More can be done with all this data than just a Bike Utilization analysis. Finding the average ride count per station can help the company predict the necessary investment in equipment and other resources. With the latitude and longitude information we can also create sections on the map and see the average ride count per day, per hour and even per day of the week for different regions. 

Also, it would be very interesting to investigate and understand the reason why the amount of male customers is much larger than female ones. Is there a way we can bring more female clients to the business? Is CitiBike doing something that is only attractive to one gender? And why this difference only applies to subscribers?

<p align="center">
<kbd>
  <img src="https://github.com/GabrielaTuma/bikesharing/blob/60253346705a1023f1860633c4b2c38ff29634e9/Images%20/Gender%20Count%20by%20UserType.png">
</kbd>  &nbsp;
</p>


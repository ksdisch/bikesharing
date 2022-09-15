# Des Moines Bikesharing Business

## Analysis Overview

### Purpose
The purpose of this analysis was to entice investors into bringing a bike-sharing program to Des Moine Iowa. To do this, I used Tableau Public to create data visualizations that show different aspects of how the bike sharing business, CitiBike, performed in New York City in August of 2019. To properly create certain visualizations, the Python Pandas library was used in Jupyter Notebook to reformat the tripduration column of 201908-citibike-tripdata.csv and change the data type to datetime, and then export a dataframe as a new csv for use in Tableau. 

### Resources
- Data Source(s): 201908-citibike-tripdata.csv, citibike_challenge_data.csv
- Tools: Tableau Public, Python, Jupyter Notebook, Pandas

## Results

### Visualizations and Description of Results

#### Duration of Checkout Times
- Original ![checkout durations](/images/checkout_durations.png?raw=true "Title")
    - Short trips are much more common than longer ones. 5 minutes is the most frequent checkout time duration, and trip durations rarely exceed 50 minutes.

#### Duration of Checkout Times by Gender
- Original ![checkout durations by gender](/images/checkout_durations_gender.png?raw=true "Title")
    - Genders follow similar checkout duration trends and males checkout the most frequently by a significant margin.

#### Customers by Gender
- Original ![customers by gender](/images/gender_distribution.png?raw=true "Title")
    - One fourth of checkouts are by females, over half are by males, and the remaining few checkouts are by those whose gender is unknown.

#### Trips by Weekday per Hour
- Original ![trips by weekday per hour](/images/trips_weekday_hourly.png?raw=true "Title")
    - Weekdays before work hours (6 - 10 AM) and after  (5-7 PM)  are frequent checkout times on weekdays. On weekends, 9 AM - 7 PM are more frequent checkout times. Thursday from 5-7 PM is the most common checkout time.

#### Trips by Gender (Weekday per Hour)
- Original ![trips by weekday per hour and gender](/images/trips_weekday_hourly_gender.png?raw=true "Title")
    - Males and females follow similar trends for which checkout times are most common. These trends are described in the Trips by Weekday per Hour visualization.

#### Trips per Weekday by Gender and Customer Type
- Original ![trips per weekday by gender and customer type](/images/trips_weekday_gender_customer_type.png?raw=true "Title")
    - Subscribers account for far more rides than regular customers for male and female genders. For those with unknown genders, regular customers account for more rides. For male subscribers, Thursday has the most rides and Sunday has the least.

#### Rides by Subscribers Vs Regular Customers
- Original ![rides by customer vs subscriber](/images/trips_customer_type.png?raw=true "Title")
    - Subscribers account for over 3/4 of total rides.

## Summary
 Some consistent themes in the analysis were that males and subscribers account for the most rides and shorter rides are much more common than long ones. This means that these groups would generate the most money for our business, which tells me two things. First, right when the business launches in Des Moines, we need to figure out ways to encourage people to subscribe. This could be running promotions, deals for referring friends, advertisements across town, and so on. Second, we need to determine how we can make the bikes more female friendly, because that is a huge demographic that we are not fully tapping in to. Finally, the fact that short rides are much more popular than long ones tells me that people are usually in a rush and/or are not traveling very far on the bikes. Because of this, we need to make the checkout process as easy and quick as possible, because if it is too much of a hassle, then people might as well walk that short distance.

### Additional Visualizations

#### Ride Counts in Less Versus More Populated/Urban Areas of NYC
Des Moines as a city is vastly different than New York City. There is less traffic, things are more spread out, there are less people, etc. However, I would like to determine the less populated areas of NYC, which come closer to simulating Des Moines than the more urban/populated areas, such as downtown Manhanttan for example. Then, I would like to compare ride counts in the less populated areas versus the more populated areas to help predict how successful ride sharing would be in Des Moines. It would be important to adjust for population size by making the metrics in the visualization, "rides per 20,000 people" for example. 


#### How Age Affects Different Metrics
New York City has a slightly older average population (36.9 years old) compared to Des Moines (34 years old). With that being said, I think visualizations examining trends associated with age would be very valuable. If checkout durations, checkout counts, etc., increase as age decreases then we can be optimistic about the potential of ride sharing in Des Moines. On the other hand, if those metrics increase as age increases, then we may need to plan for how to appeal to a younger crowd.


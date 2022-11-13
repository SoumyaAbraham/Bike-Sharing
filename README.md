# Bike-Sharing


### OVERVIEW 

As an aspiring entrepreneur trying to get ideas to materialize, the most crucial first step is doing your research. 
This project does a deep dive into multiple facets of Citibikes in New York with the hope of introducing them to Des Moines, backed by strong statistical analysis. For this research, we will be looking at the New York Citibike rides data for the month of August.

Let us go through this project and study the results of this analysis.

### ANALYSIS:

#### Step 1: Changing the datatype
We need to change the datatype for some columns in the csv file being used.  
We bring it into *pandas* and change the dataset.  

![code1](https://github.com/SoumyaAbraham/Bike-Sharing/blob/main/Screenshots/code1.png)  
![code2](https://github.com/SoumyaAbraham/Bike-Sharing/blob/main/Screenshots/code%202.png)

Note that *tripduration* datatype was *int64*.  
Using pd.to_datetime, we change the datatype to *datetime*.  
Notice that the datatype has successfully changed to *datetime64*.   
Export the new dataframe as a csv. This is what we will use for the project.  

#### Step 2: 
Connect the csv to Tableau public.  
Go on to create Tableau worksheets to visualize the data.  
Here are some of the factors we're going to analyze:  

  - Peak Hours:  
    What times are the peak hours?  
    What are the least busy hours? This information can be used to schedule maintenance times.  
  - Total Rides:  
    How many rides are in the data sample?  
  - Pie Chart of Gender Breakdown:    
    Let us see a breakdown of the customers by gender (Male, Female and Unknown).  
  - Checkout Times for Users:  
    How long do users use the Citibikes for and by how many rides?  
  - Checkout Times for Users by Gender:  
    A breakdown of the usage times by gender.  
  - Heatmap of Trips by Weekday per Hour:  
    When is the morning and afternoon rush?  
    What day of the week sees the most customers?  
    Are there any other useful trends we can see?  
  - Heatmap of Trips by Gender per Weekday:  
    A breakdown of the trip per day, focusing on usage per gender.  
    Is Citibike more popular amongst a specific gender?  
  - Heatmap of Trips by Gender per Customer Type:  
    This adds an extra layer of data, by breaking down the usage by customer type(Customer/Subscriber).  
  - Pie Chart of Customer Breakdown:  
    A pie chart of the customer types to understand the customer base.    
  - Top 10 Start Stations:  
    What are the most popular start stations and what kind of traffic do we see here?  
  - Top 10 Stop Stations:  
    What are the most popular stop stations and what kind of traffic do we see here?  
  - Start Station Map:  
    Location of each start station.
    A size and color heirarchy to see which start stations are most popular and which one see the least customers.   
  - Stop Station Map:  
    Location of each stop station.  
    A size and color heirarchy to see which stop stations are most popular and which one see least customers.  
 
*Once worksheets have been created, we will create multiple dashboards to give the data some structure. The dashboards will then be added to the Story so the data flows.*

### RESULTS:

Let us take look at the data and what they mean:

1. Peak Riding Hours
  
![Peak Riding Hours](https://github.com/SoumyaAbraham/Bike-Sharing/blob/main/Screenshots/1.%20Peak%20Riding%20Hour.png)
  
From this bar graph, we can infer the following:  

- The morning wave of peak traffic is seen between *8 AM and 9 AM*.
- The afternoon wave of the busiest hours ranges between *4 PM to 6 PM*.
- There is a considerable drop in traffic in the early morning hours, between *1 AM and 4 AM*.  
This is prime time to for maintenance work.
    
2. Checkout Times for Users
  
![Checkout Time for Users](https://github.com/SoumyaAbraham/Bike-Sharing/blob/main/Screenshots/2.%20Checkout%20Times.png)
  
From this line graph, we can see:
  
- A *5 hour* usage was the most popular time of usage by customers in August.
- By hovering over the graph, you can see the number of hours and the number of bikes that were taken out for that period of time.
    
3. Checkout Times by Gender:
  
![checkout by gender](https://github.com/SoumyaAbraham/Bike-Sharing/blob/main/Screenshots/3.%20Checkout%20Times%20by%20Gender.png)
  
This is a very informative dashboard.
  
- We see the Checkout Times by Gender, showing that there is a much *higher male clientele* than women. You will also filter the data based on the hours of the day for further analysis.
- This can be further seen in the pie chart of a breakdown of customers by Gender. 
You see only a quarter of the total customer base is female.
With a 10% unknown customer base, that shows 65% of the users being male.
- For more in-depth information, we see we are using data from 2,344,224 rides! 
    
4. Trips by Day of the Week per Hour
  
![trips by weekday](https://github.com/SoumyaAbraham/Bike-Sharing/blob/main/Screenshots/4.%20Trips%20by%20Weekday%20per%20Hour.png)
  
What we see here is:
  
- *Thursdays* are the busiest day of the week, closely followed by Monday and Tuesday. 
- *8 AM* in the morning and *5PM to 6 PM* in the evening are the busiest on most days.
- On weekends, we see a more even distribution of customers between *10 AM to 7 PM*, with Saturday being the busier of the two.

    
5. Trips by Gender per Day
  
![gender per day](https://github.com/SoumyaAbraham/Bike-Sharing/blob/main/Screenshots/5.%20Trips%20by%20Gender%20per%20Day.png)
  
With this heatmap, we can see the busiest hours per day, further divided by Gender.
- Once again, we can see that *8 AM* is the busiest hour in the mornings, with a *much higher number of male users*.
- The busiest hours of the afternoon is between *5 PM and 6 PM.*
- This map shows that *Thursdays* are the busiest day of the week.
- You can also *filter the heatmap by gender*.

    
6. Trips by Gender per Customer Type
  
![gender type by customer](https://github.com/SoumyaAbraham/Bike-Sharing/blob/main/Screenshots/6.%20Trips%20by%20Gender%20per%20Customer%20Type.png)
  
Here is a further breakdown of the previous heatmaps to tell us 
- Citibikes are used much *more by Subscribers than by customers*.
- *Male subscribers* use Citibikes much more than female subscribers.
- The *weekends* are when customers are more likely to use Citibikes.  
- You have the option of narrowing your analysis by *filtering data by gender or customer type.*
    
On your right is a pie chart to show that less than a quarter of the Citibike customer base are *Non-Subscribed* customers.
  
7. Top 10 Start Stations

![top 10 start stations](https://github.com/SoumyaAbraham/Bike-Sharing/blob/main/Screenshots/7.%20Top%2010%20Start%20Station.png)

We have two visual aids in this dashboard. 
On the left, we have a bar graph showing us the most populat starting stations with their ride counts.  
On the right, we have a map with a marker representing each Start Station. 

8. Top 10 Start Stations

![top 10 stop stations](https://github.com/SoumyaAbraham/Bike-Sharing/blob/main/Screenshots/8.%20Top%2010%20Stop%20Station.png)

Once again, we have two visual aids in this dashboard. 
On the left, we have a bar graph showing us the most popular stopping stations with their ride counts.  
On the right, we have a map with a marker representing each Stop Station. 

The marker size and color intensity increase as the ride count at these stations increase.
This helps us see what the more popular locations are.   

*We can further do a deep dive to see what factors could be contributing to this ride count to get a better understanding of how this information can translate to station selection in Des Moines.*

### Summary:

Given this information, we learn trends that will be important to keep in mind when starting out in Des Moines.

- What type of Customer Base is most popular? 
- What times of the day does Des Moines experience the office rush? It is likely to coincide with that of bike usage.
- It is possible that a particular gender is more prone to use Citibikes. In New York, it was seen to be more popular with Males. Try to find out why this is and how the experience can be improved to appeal to all genders.
- Is there a particular day of the week that sees more bike traffic? Could this correlate with the new Hybrid work system that is being globally accepted?
- What factors affect the most/least popular starting and ending stations? What locations in Des Moines equate to these? 
- It is important to keep in mind that New York City sees a very high amount of tourists and out-of-towners, especially on weekends. Also, the subway systems in NYC is also very popular among commuters. When charting your expectations, take this into account. Are there other popular means of transport in Des Moines? What does the tourism sector look like in Des Moines?

Answering these questions will get you one step closer to seeing your ideas take flight!

In case you would like to access the project dashboard, you can find it [here](https://public.tableau.com/app/profile/soumya.abraham/viz/Citibikes_DesMoineChallenge/Citibikes_NYC?publish=yes)  
You can also find the python code to change datatypes [here](https://github.com/SoumyaAbraham/Bike-Sharing/blob/main/NYC_CitiBike_Challenge.ipynb)

# Bay_wheels_exploration
Bay Wheels is a regional public bicycle sharing system in the San Francisco Bay Area, California owned by Lyft. Beginning operation in August 2013 as Bay Area Bike Share. Here we collect, clean and analyse their 2019 trip data, Answer 5 major questions regarding the business growth using matplotlib and seaborn libraries to develop visualize insights
### Bay Wheels Bike 2019 Data 
Bay wheels Bike data, the data had 2506983 entries. Features:
The data had features like user type, which share details about the type of user, whether they are subscribed or just random customers accessing bike usage. The data also had features like type of bike access, whether by app or clipper, company also provide an offer of bike share, a plan where users gets 24/7 bike usage with annual fee of $5.

Major questions to be answered:

1. Find the time period where campaigns should be started to attract more customers to subsribe to the application?  
2. Proportion of the customers using application, does the subscribers prefer using application or clipper for renting bikes?
3. Analyze the surge hours during a day, so that we need to ensure that customers are met with the need.  
4. Customer target: Is there a specific customer target to be generated, like tourists, whitescholors etc?  
5. Is the new feature bikeshare a success?, discuss the effort needed to attarct more customers to bike share plan.  
These questions are answered using exploratory analysis:

## Data Collection
WE have 12 csv files, which are downloaded using request library, and stored in a file location
```
path = r'ford_bike_data'
all_data = glob.glob(os.path.join(path, "*.csv"))
```




##### Univariate exploration:
From 'month bike ride usage' we could see that number of customers using the bikes see an increase during march and april, so this is the time we could start campaigns to attract more customers to bike usage. This graph answers our first question about the time period during an year where campaigns to be initiated. Univariate analysis also discuss about bike rides during week in 'Bike rides during Weekdays' plot, where we could see bike usage is heavy during weekends whereas usage reduce to half during weekends

##### Bivariate exploration:
'Bike rides during a day by user-type' analyze the surge hours during a day for bike usage and finds the answer for the third question, it can be seen that from 7am to 10 am and 4 pm to 7 pm we see a surge in bike usage. Comparing it to the plot 'User_type based on weekday bike usage' we could say office hours or whitescholors are our major customer target, as we could see that during weekdays we have more of the subsribers using bikes, and they can be working profesionals.

##### Multivariate exploration:
'Subscribers monthly bike rides by rental bikes', shows us subscribers prefer using application, which is good, usage of clipper is said to be low in both the type of users. 'Subscribers monthly bike rides by bike share' plot shows that most of the subscribers haven't opted for share bikes plan. So this plan needs improvement as throughout the year the users remained the same.


# Bay_wheels_exploration
Using matplotlib and seaborn library to analyse Bay wheels company data, and visualize insights
### FordGo Bike Data 
For data analysis I consider 2019 Ford Gobike data, the data had 2506983 entries. Features:
The data had features like user type, which share details about the type of user, whether they are subscribed or just random customers accessing bike usage. The data also had features like type of bike access, whether by app or clipper, company also provide an offer of bike share, a plan where users gets 24/7 bike usage with annual fee of $5.

Major questions to be answered:

1. Find the time period where campaigns should be started to attract more customers to subsribe to the application?  
2. Proportion of the customers using application, does the subscribers prefer using application or clipper for renting bikes.
3. Analyze the surge hours during a day, so that we need to ensure that customers are met with the need.  
4. Customer target: Is there a specific customer target to be generated, like tourists, whitescholors etc.  
5. Is the new feature bikeshare a success, discuss the effort needed to attarct more customers to bike share plan.  
These questions are answered using exploratory analysis:

##### Univariate exploration:
From 'month bike ride usage' we could see that number of customers using the bikes see an increase during march and april, so this is the time we could start campaigns to attract more customers to bike usage. This graph answers our first question about the time period during an year where campaigns to be initiated. Univariate analysis also discuss about bike rides during week in 'Bike rides during Weekdays' plot, where we could see bike usage is heavy during weekends whereas usage reduce to half during weekends

##### Bivariate exploration:
'Bike rides during a day by user-type' analyze the surge hours during a day for bike usage and finds the answer for the third question, it can be seen that from 7am to 10 am and 4 pm to 7 pm we see a surge in bike usage. Comparing it to the plot 'User_type based on weekday bike usage' we could say office hours or whitescholors are our major customer target, as we could see that during weekdays we have more of the subsribers using bikes, and they can be working profesionals.

##### Multivariate exploration:
'Subscribers monthly bike rides by rental bikes', shows us subscribers prefer using application, which is good, usage of clipper is said to be low in both the type of users. 'Subscribers monthly bike rides by bike share' plot shows that most of the subscribers haven't opted for share bikes plan. So this plan needs improvement as throughout the year the users remained the same.


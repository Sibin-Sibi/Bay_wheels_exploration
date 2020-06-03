# Bay_wheels_exploration
Bay Wheels is a regional public bicycle sharing system in the San Francisco Bay Area, California owned by Lyft. Here we collect, clean and analyse year 2019 trip data, answer 5 major questions regarding the business growth using matplotlib and seaborn libraries to develop visualize insights
### Bay Wheels Bike 2019 Data
[Bay Wheels Data](https://www.lyft.com/bikes/bay-wheels/system-data) data have 2506983 entries. 
Features:
The data had features like user type, which share details about the type of user, whether they are subscribed or just random customers accessing bike usage. The data also had features like type of bike access, whether by app or clipper, company also provide an offer of bike share, a plan where users gets 24/7 bike usage with annual fee of $5.

Major questions to be answered:

1. Find the time period where campaigns should be started to attract more customers to subsribe to the application?  
2. Proportion of the customers using application, does the subscribers prefer using application or clipper for renting bikes?
3. Analyze the surge hours during a day, so that we need to ensure that customers are met with the need.  
4. Customer target: Is there a specific customer target to be generated, like tourists, whitescholors etc?  
5. Is the new feature bikeshare a success?, discuss the effort needed to attarct more customers to bike share plan.  
These questions are answered using exploratory analysis:

## Data Collection
We have 12 csv files, which are downloaded using request library, and stored in a file location, these files are joined using glob module, which retrieves file from the path. 'OS' module helps in interacting with python.
```
path = r'ford_bike_data'
all_data = glob.glob(os.path.join(path, "*.csv"))
```
After assesment, data is cleaned. and we perform various visualization using matplotlib and seaborn to anwer the questions, some of the visualizations are shown below

##### Univariate exploration:
![1](https://user-images.githubusercontent.com/60280080/83698987-e4e1b800-a5d0-11ea-8810-4b29b060a952.JPG)

From 'month bike ride usage' we could see that number of customers using the bikes see an increase during march and april, so this is the time we could start campaigns to attract more customers to bike usage. This graph answers our first question about the time period during an year where campaigns to be initiated. Univariate analysis also discuss about bike rides during week in 'Bike rides during Weekdays' plot, where we could see bike usage is heavy during weekends whereas usage reduce to half during weekends

##### Bivariate exploration:
![2](https://user-images.githubusercontent.com/60280080/83699064-15c1ed00-a5d1-11ea-80e2-49f1603dfb53.JPG)

'Bike rides during a day by user-type' analyze the surge hours during a day for bike usage and finds the answer for the third question, it can be seen that from 7am to 10 am and 4 pm to 7 pm we see a surge in bike usage. Comparing it to the plot 'User_type based on weekday bike usage' we could say office hours or whitescholors are our major customer target, as we could see that during weekdays we have more of the subsribers using bikes, and they can be working profesionals.

##### Multivariate exploration:
![3](https://user-images.githubusercontent.com/60280080/83699125-43a73180-a5d1-11ea-8d57-7c00f24fa3a4.JPG)

'Subscribers monthly bike rides by rental bikes', shows us subscribers prefer using application, which is good, usage of clipper is said to be low in both the type of users. 'Subscribers monthly bike rides by bike share' plot shows that most of the subscribers haven't opted for share bikes plan. So this plan needs improvement as throughout the year the users remained the same.


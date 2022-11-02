# Data_Project (Bellabeat Case Study)
Projects that involve hands-on use of data analytics tools such as SQL, Excel, R, Tableau and more. 

bellabeat_logo Bellabeat is a fictional manufacturer of health-focused technology products for women. Founded in 2013 and now a successful small company, Bellabeat wants to expand further into the global smart device market. The company currently offers several smart device products including a wellness tracker, a smartwatch, and smart water bottle, and an app to connect to these smart products and manage user data. Bellabeat offers a subscription-based membership for users to access fully personalized guidance on nutrition, activity, sleep, and mindfulness based on their lifestyle and goals.
Stakeholder Goals

In order to better inform Bellabeat's marketing strategy, the company's cofounder and Chief Creative Officer would like to understand how consumers use smart devices across the market and find out how that may translate to the way Bellabeat consumers use their devices. They want to understand the following:

1. What are some trends in smart device usage?
2. How could these trends apply to Bellabeat customers?
3. How could these trends help influence Bellabeat marketing strategy?
Data

The dataset is made up of external data not provided by Bellabeat. It is a series of observations of 33 individual fitness device users from which the Bellabeat marketing team hopes to extrapolate information about its own consumers. 

To approximate this data, this case study is an analysis of a public datset of 33 individuals whose activity was recorded by their Fitbit devices over a period of two months. This data provides users' calories burned, activity intensity, step count, and sleep behavior, aggregated over days, hours and minutes. This dataset can be found here.

To better focus this analysis we will look for trends in user data across fitness level, general useage, and step count aggregated daily. We will also look for activity trends throughout the day, such as whether users are more active in the morning or evening.

Limitations

30 users is the lower threshold for the sample size of a study whose results have statistical significance. Ideally, the data team would find and study a dataset with a higher number of users so as to avoid sampling bias. 

Additionally, some of the provided data, such as the weight log files, are unusable for analysis due to user inconsistency. Out of 33 users, only 2 were consistent in manually adding their daily weight to the app throughout the 30 day sampling period, so unfortunately this analysis will be unable to provide insights on how fitness tracker wearers may be using their devices for weight loss. 


Data Preparation

For the most straightforward analysis, data was arranged according to granularity. Daily data (activity level, daily steps, sleep hours) was compiled together and hourly data was analyzed separately to assess trends across users throughout the day. This analysis will focus on overall user habits over days and hours, rather than the more granular minute-by-minute observations recorded by the fitness device. 

Data was inspected, organized, and cleaned in Microsoft Excel before being loaded into Tableau for visualization.

Analysis

For the purposes of this analysis, the question of searching for trends across the user base is extremely broad: this warrants more discussion of the stakeholder's goals and interests. However, for now, there are a number of interesting data points here. For example, in the daily data we can look at the date, total steps, total distance, distance over activity type, minutes of activity type, calories burned, minutes asleep, and minutes in bed. Some further questions I'll try to answer in regards to everyday use of the fitness tracker are: 

Q: How much time do users spend doing activities throughout the day? 
A: Users spend 81% of the day sedentary, 16% of the day lightly active, 1% of the day fairly active and 2% of the day very active.

Q: Do users prefer rigorous workouts or more lowkey forms of exercise like walking? 
A: Based on the distribution of activity preferences, we can conclude that most workout-type activity undertaken by users is in the lightly active category (walking, pilates, yoga).

Q: Are users more active in the morning, afternoon, or evening?
A: Users are more active in the afternoon and early evening, with the two peak activity times being 12pm-2pm and 5pm to 7pm.

Q: What range of activity level was observed among participants?
A: Users ranged from an average of 916 daily steps to 16,040 daily steps. 

Q: Does the user pool contain more sedentary, lightly active, fairly active, or very active users?
A: Based on step count data, the user pool largely favors lower activity levels, with 24% considered sedentary, 27% lightly active, 27% somewhat active, 15% active, and 6% very active.
Discussion

This dataset has been visualized as an interactive dashboard in Tableau which can be accessed here.


resize-dash

Initial analysis of user activity shows that users are primarily sedentary when wearing fitness devices. The average user is sedentary for 81% of the day, lightly active for 16% of the day, anf fairly or very active for 1% and 2% of the day, respectively. This observation makes logical sense, since sleep takes up one third of a 24-hour period and users are likely wearing their devices all the time. Many users may additionally have sedentary office or administrative jobs, which could account for the remainder of inactive time.

Eliminating sedentary time from the analysis gives a better picture of what type of activity users prefer when they choose to work out: light activity, moderate activity, or very active (rigorous) activity. Users clearly have a preference for light activity like walking, yoga, or pilates. These exercises are almost universally beneficial, low-impact, and easy to incorporate into one's daily routine. These are good options for people seeking to build a more active lifestyle, especially for those exploring how to live more healthfully for the first time. Interestingly, more rigorous workouts (like running, kickboxing, or HIIT) are the next most popular workout type and make up nearly 10% of user activity outside of sedentary behavior.

Analysis of average daily step count over a 24 hour period serves as a measure for what time of day users prefer to be active. The two most popular times of day for users to be active are in the middle of the day (perhaps on lunch break from work) and immediately after the workday, with the highest average user activity recorded during the 6:00pm hour. Users were rarely active during the late night and very early morning hours when people are usually asleep. Overall activity records reflects a diurnal circadian rhythm, with users moving around during the daylight hours generally, and peak activity points during the lunch hour (noon to 2pm) and immediately after work (5pm to 7pm).

Regarding the range of average step counts across the entire user pool: the user with the highest average step count took 16,040 steps per day and the user with the lowest average step count took only 916 steps per day. The median user took 7,283 steps per day on average. The most popular day for users to be active was Saturday, with an average of 344 steps across the user pool. The least popular day for activity was Sunday, with 288 steps on average among users.

Step counts were aggregated by using the recommendations found here to classify users according to their activity levels. Users overall tended to favor the less active portion of the spectrum of activity, with 24% of users considered sedentary (<5,000 average daily steps), 27% lightly active (5,000 to 7,499 steps), 27% somewhat active (7,500 to 9,999 steps), 15% active (>10,000 steps) and 6% very active (>12,500 steps).

Recommendations

The above trends in how consumers use wearable fitness devices (FitBit) provides substantial insight into how Bellabeat customers might use their devices. Based on these findings, some recommendations for the Bellabeat marketing team are:

Provide some social aspect of the app so that users can connect (or compete!) with friends to improve step counts and achieve fitness goals.
Issue discount codes for users to invite their friends to buy Bellabeat products and get fit together.
Keep track of users' overall activity levels and celebrate when a user moves into a higher category (ie from sedentary to lightly active).
Push step count reminders to users on days and times when they are already likely to want to be active: Saturdays and weekdays after work.
Reward users who consistently meet daily and weekly step count goals.
For users who are interested in weight loss, perhaps the introduction of a digital scale that pairs with the Bellabeat device via Bluetooth would help users stay consistent about tracking their weight and remove the barrier of needing to add this data to the device manually.

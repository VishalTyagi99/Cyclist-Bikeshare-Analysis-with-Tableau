## 📝 Introduction
The Cyclistic Bike Share Case Study is a capstone project for the Google Data Analytics Professional Certificate on Coursera. In this project, I will follow the data analysis process which I learned from the course: ask, prepare, process, analyze, share and act to analyze the data.
## 💬 Background
### Cyclistic
Cyclistic is a bike-share company based in Chicago that launched a successful bike-sharing program in 2016. Throughout the years, the program has expanded significantly to a fleet of 5,824 bicycles and a network of 692 geotracked stations sprawled across the city. With the large number of bicycles across numerous stations, customers can rent bikes from one station and return them to any other station within the network at their convenience. This encourages people to opt for cycling as a mode of transportation, therefore contributing to the success of Cyclistic's bike-sharing program.

Cyclistic's marketing strategy has so far focused on building general awareness and appealing to broad consumer segments. The company offers flexibile pricing plans that cater to diverse needs of users including single-ride passes, full-day passes, and annual memberships. Besides, it provides reclining bikes, hand tricycles, and cargo bikes, effectively welcoming individuals with disabilities and those who can't ride on the standard two-wheeled bicycles. Based on the company database, Cyclistic users are more likely to ride for leisure, but about 30% use them to commute to work each day. While traditional bikes remain as the popular option, around 8% of users opt for the assistive alternatives.

The company's marketing director believes that the company’s future success depends on maximizing the number of annual memberships. Therefore, as a junior data analyst, my team and I have to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, we will design a new marketing strategy to convert casual riders into annual members.
### Scenario
I am assuming to be a junior data analyst working in the marketing analyst team at Cyclistic, a bike-share company in Chicago. The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, my team wants to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, my team will design a new marketing strategy to convert casual riders into annual members. But first, Cyclistic executives must approve our recommendations, so they must be backed up with compelling data insights and professional data visualizations.
## ⚙ Approach/Steps
### 1. Ask
### Business Task- design marketing strategies to convert casual riders to members by understanding how annual and casual riders differ, why casual riders would buy a membership, and how digital media could affect their marketing tactics.
### Analysis Questions
Three questions will guide the future marketing program:

1.How do annual members and casual riders use Cyclistic bikes differently?
2.Why would casual riders buy Cyclistic annual memberships?
3.How can Cyclistic use digital media to influence casual riders to become members?
### 2. Prepare
### Data Source: Trip data 
[Note that the data has been made available by Motivate International Inc. under this license.]
### Tools:
- Data cleaning & processing - SQL on Google Big Query
- Data visualization - Tableau
### 3. Process
1.Data Exploration
2.Data Cleaning
3.Data Analysis
### Data Exploration
I ran the queries for each column from left to right in order to determine the data type and to uncover any missing values, outliers, inconsistencies, and errors within the dataset.

The data set consists of 13 variables, as shown in the following:
|No.| Variable | Description |
|---| --- | --- |
|1|ride_id| Unique ID assigned to each ride |
|2|rideable_type| classic, docked, or electric
|3|started_at|	Date and time at the start of trip
|4|ended_at|	Date and time at the end of trip
|5|start_station_name|	Name of the station where the ride journey started from
|6|start_station_id|	ID of the station where the ride journey started from
|7|end_station_name|	Name of the station where the ride trip ended at
|8|end_station_id|	ID of the station where the ride trip ended at
|9|start_lat|	Latitude of starting station
|10|start_lng|	Longitude of starting station
|11|end_lat|	Latitude of ending station
|12|end_lng|	Longitude of ending station
|13|member_casual|	Type of membership of each rider
### Data Cleaning
Before analyzing the data, the dataset was cleaned by:

- Removing the trips with null values.
- Adding 3 columns: 'ride_length_in_mins', 'day_of_week' and 'month'.
- Exclusing the rides with duration less than a minute or longer than a day.
In total, 4,224,062 rows were returned, which means 1,443,655 rows were removed.
### 4. Analyze
### Data Analysis
The analysis question is:
- How do annual members and casual riders use Cyclistic bikes differently?

The cleaned data is imported into Tableau for analysis and the figures plotted are displayed in the following.
 ### Total Rides in 2022
 The figure below shows the total number of rides carried out by Cyclistic members and casual riders in 2022.
 ![Cyclistic Bike Share Case Study  -  Protected View - PowerPoint 14-03-2024 16_45_00](https://github.com/VishalTyagi99/Cyclist-Bikeshare-Analysis-with-Tableau/assets/127587576/631044ba-2d7a-4a7e-bccb-f27512310281)
- Cyclistic members recorded a greater bicycle activity than casual riders. The total rides for Cyclistic members are 2,511,003 while 1,713,059 trips for casual riders.
- Cyclistic members accounted for about 59.4% of total rides whereas casual riders made up 40.6% of total rides in 2022.
 ### - Types of Bikes
 The types of bicycles used for the trips are displayed as follow:
 ![Cyclistic Bike Share Case Study  -  Protected View - PowerPoint 14-03-2024 16_45_32](https://github.com/VishalTyagi99/Cyclist-Bikeshare-Analysis-with-Tableau/assets/127587576/967a5274-1a27-4161-8e79-011a108ad9ec)
- There are three types of bicycles: classic, electric and docked bikes.
- Cyclistic members and casual riders prefer show a higher preference for classic bicycles over electric bicycles.
- Casual riders have also used the docked bicycles.
###  Average Ride Duration
The average ride length is plotted against the type of users (member vs. casual):
![Cyclistic Bike Share Case Study  -  Protected View - PowerPoint 14-03-2024 16_45_55](https://github.com/VishalTyagi99/Cyclist-Bikeshare-Analysis-with-Tableau/assets/127587576/2d120e7f-f03b-4e22-a98e-b0c5c923efa2)
- Cyclistic members can ride on the bicycles for about 12.41 minutes on average whereas casual riders have an average ride length of 23.82 minutes. Hence, the ride duration of Cyclistic members are approximately two times smalelr than casual riders.
### - Trips Taken in a Month
The preference of cycling activity can be determined by drawing the graph of trips taken against month from January to December 2022.
![Cyclistic Bike Share Case Study  -  Protected View - PowerPoint 14-03-2024 16_46_04](https://github.com/VishalTyagi99/Cyclist-Bikeshare-Analysis-with-Tableau/assets/127587576/8176dac4-4bba-4d41-a263-0239319ea5ee)
- Both Cyclistic members and casual riders have the lowest activity, 65,051 rides and 12,355 rides respectively in January 2022.
- Cyclistic members have the highest activity (323,073 rides) in August 2022.
- Casual riders have the greatest activity (303,273 rides) in July 2022.
###  Average Ride Length in a Month
The mean trip duration is depicted in the line graph below.
![Cyclistic Bike Share Case Study  -  Protected View - PowerPoint 14-03-2024 16_45_59](https://github.com/VishalTyagi99/Cyclist-Bikeshare-Analysis-with-Tableau/assets/127587576/f1a89d3b-6efc-4cf0-b51b-cefc3be5d3d6)
- The monthly average ride duration for Cyclistic members is the highest in June (13.65 minutes).
- For casual riders, the highest mean trip duration is in May (27.75 minutes).
 ### Trips Taken in a Week
 The bar chart below is used to study the daily user activity over a week.
![Cyclistic Bike Share Case Study  -  Protected View - PowerPoint 14-03-2024 16_46_07](https://github.com/VishalTyagi99/Cyclist-Bikeshare-Analysis-with-Tableau/assets/127587576/937bc1f9-1b3e-42d9-8b4e-86f10f34b72d)
- Generally, bike rides are most frequented on Saturdays.
- Cyclistic members have the highest activity (399,863 rides) on Thursdays while the lowest activity (286,128 rides) on Mondays.
- Casual riders have the greatest activity (357,781rides) on Saturdays while the least activity (191,467 rides) on Tuesdays.
### Average Ride Length in a Week
The mean ride duration across the week is displayed as follow.
![Cyclistic Bike Share Case Study  -  Protected View - PowerPoint 14-03-2024 16_46_01](https://github.com/VishalTyagi99/Cyclist-Bikeshare-Analysis-with-Tableau/assets/127587576/15360bdf-237e-4959-b0e2-02c97d857eec)
- Cyclistic members cycled the longest on Saturday with an average ride length of 14.01 minutes.
- On the other hand, casual riders cycled the longest on Sunday with a mean trip duration of 27.18 minutes.
### 5. Share
![Cyclistic Bike Share Case Study  -  Protected View - PowerPoint 14-03-2024 16_46_14](https://github.com/VishalTyagi99/Cyclist-Bikeshare-Analysis-with-Tableau/assets/127587576/4603c373-b32c-4f7c-bc8f-767a7a81a36d)
The similiarities and differences between Cyclistic members and casual riders were drawn from the dashboard above.
### Similarities:
- Both Cyclistic members and casual riders prefer riding bicycles in the spring and summer seasons (from May to September). However, the number of rides decrease since September. This may be due to change of season in which the weather temperature drops and becomes uncomfortable for rides.
- Both Cyclistic members and casual riders prefer classic bicycles over electric bicycles.
- Both Cyclistic members and casual riders have higher average ride duration on weekends as compared to on weekdays
### Differences:
- Cyclistic members go on more rides than casual riders.
- Cyclistic members have smaller average ride length (12.41 minutes) than casual riders (23.82 minutes). Hence, this may suggest that the Cyclistic members take the bicycles for short trips or short distance travel.
- Cyclistic members show consistent rides throughout the week while casual riders have the busiest activites on weekends and lowest activities during weekdays. This may indicate that the Cyclistic members use the bicycles for *purpose-oriented rides such as work or errands while the casual riders use bicycles for leisure or recreational activities.
### 6. Act
### Recommendations
From the analysis above, we can design marketing strategies to convert casual riders to Cyclistic members. Here are my suggested approach:

- ### Membership Personalisation
Provide a range of membership personalizations: yearly, monthly and daily. For example, $365/year, $45/month, $3/day. Users will be able to choose their membership type according to their own preferences. By introducing shorter-term membership plans with appropriate pricing, we can cater the needs of riders who might not need an annual membership.

- ### Group Membership Discounts
Offerdiscounted plans for friends, students, and families can encourage collective memberships. Furthermore, it encourages users to cycle together and strengthen the bonds between people.

- ### Membership Loyalty Points System
Implement a membership loyalty points system for users to collect points for each ride. Rewards such as membership discount will be given based on the number of points collected. This will encourage riders to use the service more frequently, driving engagement and loyalty.

- ### Member-Exclusive Events
Organize member-exclusive events such as group rides, urban exploration challenges, or themed cycling events. This approach not only encourages more rides from current members but also entices casual riders to join as members to participate in these unique experiences.

- ### Seasonal campaigns
Launch seasonal campaigns by offering limited-time discounts, special weekdays offers, or extended ride durations for members during these seasons to help in making the service more sustainable and manageable.

- ### Social Media Engagement
Utilize digital media, including social media platforms, to engage with both casual riders and potential members. Share success stories, testimonials, and user-generated content from Cyclistic members who have benefited from the membership. Create visually appealing content showcasing the joy of cycling during different seasons and scenarios, enticing casual riders to become members.
## 🔮 Conclusion
In short, this analysis provides valuable insights into the preferences and behaviors of Cyclistic members and casual riders. By tailoring strategies to the identified differences and preferences, Cyclistic can effectively convert casual riders into portential members.




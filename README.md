# Divvy-Bike-Sharing-Analysis-Q1-2020
##Uncovering Ridership Patterns in Chicago

- Table of Contents
- Project Overview
- Data Sources
- Tools Used
- Data Cleaning/Preparation
- Exploratory Data Analysis
- Data Analysis
- Results/Findings
- Recommendations
- Limitations
- References

##Project Overview

The goal of this project was to analyze the Divvy bike-sharing service in Chicago for the first quarter of 2020. By examining the trip data, I aimed to understand the differences in usage patterns between annual members and casual riders. The key objectives were to identify trends in ride duration, popular stations, and peak usage times to provide actionable insights for:
1. A marketing strategy focused on converting casual riders into members.
2. Resourse Allocation
3. Operational Improvements

##Data Sources

The analysis is based on the Divvy_Trips_2020_Q1.csv dataset, Publicly available bike share data from the Divvy system.

Tools Used
Google Sheets: For data cleaning, transformation, and initial analysis.
Tableau: For creating the interactive dashboard and visualizing the findings.
Data Cleaning/Preparation
The raw data required several preparation steps to be ready for analysis. The process included:
Checking for and removing any duplicate entries.
Ensuring there were no null values in critical columns like ride_id, started_at, and ended_at.
Calculating the trip_duration in minutes for each ride by finding the difference between ended_at and started_at timestamps.
Extracting the month and day of the week from the started_at timestamp to facilitate time-based analysis.
Exploratory Data Analysis
My initial exploration focused on getting a high-level understanding of the dataset. I looked at the overall distribution of trips, comparing the total number of rides between members and casual riders. I also identified the range of trip durations and noted the primary type of bike used, which was the "docked bike." This phase helped shape the more detailed questions I would ask during the main analysis.
Data Analysis
In this phase, I delved deeper into the usage patterns. A key part of the analysis was aggregating data to compare the two user types across different dimensions.
One interesting feature was calculating the average trip duration for each user type and for each day of the week. This required grouping the data and applying aggregate functions, which I accomplished using functions and Pivot Tables within Google Sheets. For example, to find the average trip duration per user type, I used functions like AVERAGEIF to calculate the average where the user type was "member" or "casual".
This allowed me to see that casual riders, on average, take significantly longer trips than members, suggesting different use cases (e.g., leisure vs. commuting).
Results/Findings
The analysis and visualization led to several key findings, as summarized in the dashboard.
Total Rides: There were approximately 424,000 rides in Q1 2020.
User Breakdown: Annual members are the dominant user group, accounting for a large majority of the rides.
Average Trip Duration: The average trip duration was 17.15 minutes. However, this varies greatly between user types, with casual riders having much longer average ride times.
Monthly Trends: Usage increased each month, with March having the highest ridership of the quarter.
Weekly Trends: Ridership is fairly consistent throughout the week, with a slight peak during typical commuting days (Monday-Friday).
Popular Stations: The most frequented start and end stations are concentrated in downtown areas, such as near Lake Shore Drive, Michigan Ave, and Canal St, indicating strong commuter and tourist activity.
Recommendations
Based on the findings, I propose the following recommendations:
Targeted Membership Campaigns: Launch marketing campaigns aimed at casual riders who take frequent, long trips. Offer them a discounted first-year membership to highlight the cost savings over paying per ride.
Optimize Station Capacity: Increase the number of available bikes at the top 5 most popular start/end stations during peak weekday hours to meet commuter demand.
Weekend Promotions: To boost weekend usage among members and attract more casual riders, introduce special weekend promotions or suggest scenic leisure routes starting from popular stations.
Limitations
This analysis is subject to a few limitations:
Seasonality: The data only covers the first quarter (winter months). Rider behavior is likely to be very different in warmer seasons.
COVID-19 Impact: The data from late March 2020 may reflect the early impacts of the COVID-19 pandemic, which could skew typical ridership patterns.
Lack of Demographics: The dataset is anonymized, so it's not possible to analyze usage patterns based on user demographics like age or gender.
References
Divvy Trip Data (2020). Lyft Bikes and Scooters, LLC. Retrieved from https://divvy-tripdata.s3.amazonaws.com/index.html

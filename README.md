# Bike Share Analysis 

## Project Background
Launched in 2016, Cyclistic is a successful bike-sharing company that has expanded its services and marketing initiatives over the years. While the business is established, there is potential to maximize revenue by increasing the number of members, who are the company’s primary source of income. Cyclistic collects detailed data on both casual users and members, including their activity patterns on the service.

This project uses Excel to analyze bike-share data with the goal of uncovering the key differences between casual users and members. The insights gained aim to inform strategies that can boost membership adoption and revenue. 

## Executive Summary 
This project analyzes over 1M bike-share rides from Cyclistic to compare member and casual users. Key findings show members make up 75% of trips and primarily ride for weekday commutes, while casuals ride on weekends and afternoons for leisure. Recommendations include introducing flexible membership options, launching seasonal campaigns, and partnering with businesses to boost member adoption.

## Data Description 

The source of the data examined in this project is Cyclistic; the analysis covers 12 months of data from December 2024 to November 2025. Combined, this dataset consists of over 1 million riders and 13 features describing each rider's trip. Due to Excel's row limit, the summer months were excluded, and 7 months were examined, including January, February, March, April, October, November and December. 

### Key Feature / Columns
- **ride_id**: A unique identifier for each ride
- **rideable_type**: Type of bike, classic or electric
- **started_at/ended_at**: The time and date of when the ride started and ended
- **member_casual**: Membership status of rider

## Methadology 
The 12 months of data were derived from monthly CSV files, which were imported to Power Query. The files were merged into a single dataset once the initial transformation of the organization was conducted using Power Query. While Power Query aided in the alignment and initial organization of data, there were still some discrepancies, as well as further preparation required to set up for the analysis. These steps consisted of the following:

- Removed unused station columns due to null values 
- Filtered the membership column to only include "member" and "casual" 
- Removed duplicate rows as well as blank rows
- Created new calculated fields: ride duration, ride bins (time of day, ride length), day/month/hour extracted from start_at

## Analysis
During the analysis process, the primary tool used was pivot tables. By using pivot tables, over 1 million rows of data were efficiently organized into actionable insights. 

### Total Membership Split 
It was discovered that out of the million rider data, 25% of these riders were casual users, while the majority of 75% users were members. This reinforces the claim that the business is successful in its current efforts, but needs slight tweaks to convert the remaining 25% of users. 

### Weekly Trends 
When analyzing the line graph for the trends of users throughout the week, it was apparent that casual users have higher usage on the weekends, whereas members have higher usage during weekdays. This indicates that casual users are more likely to use this service for leisure, whereas members may use it as a means of commuting to work.

### Time of Day Trends
The analysis of this factor suggests that the majority of casual users use the bike service between hours of 12 pm and 4 pm, which is the afternoon. However, members use this service most between hours 5 pm and 8 pm, which is the evening. This insight reaffirms our former conclusion that most members use the bike-share for work commute, whereas casual users use it for leisure. 

### Ride Length Trends
The results of comparing the length of rides for each membership were not a significant differentiator between casuals and members, suggesting that the trip purpose (commute vs leisure) is more influential than trip duration. 
### Monthly Trends
While the results of both members' usage across a year were in consensus, there were some valuable insights. There is a spike in April that aligns with what one may assume as the weather is warmer; consequently, in colder months, there is lower usage as is inevitable. Due to Excel’s row limit, July–September were not included. Based on April/May growth, we can reasonably infer summer peaks, but this should be validated with the full dataset.
 
## Reccomendations 
Based on the uncovered insights, the following recommendations have been provided:
- **Versatile membership options:** The majority of casual users use this service on the weekend for leisure; this means that getting an annual membership is not feasible. This means that, rather than having only two options for membership, there should be more accommodations. A beneficial option would be to add a weekend membership that allows those who do not use the bike-share during the weekdays to commit to an annual membership for just the weekends. 
- **Seasonal campaigns:** During the warmer seasons, there is a general spike in business. These seasons also result in an increased number of tourists, for which a summer membership would be ideal. A summer membership would mean that casual members would be more comfortable committing, and after analyzing their trip patterns over the summer, they could receive a personalized offer. For example, if they are a tourist, they could receive a discounted price next time they visit, increasing the number of loyal users. Similarly, a local could receive incentives for extending their membership, such as a discounted price for the following months. 
- **Collaborate with businesses:** It is important to market in areas where the target audience would be most. This includes corporate settings encouraging more activity and having on-site bike-share stations, as well as marketing at local gyms and coffee shops. By partnering with businesses such as local coffee shops, you can include their items as part of your loyalty rewards program. This not only serves as an incentive for users but also improves marketing efforts and partnerships.


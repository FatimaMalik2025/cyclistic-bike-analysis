# Bike Share Analysis 

## Project Background
Launched in 2016, Cyclistic is a successful bike-sharing company that has expanded its services and marketing initiatives over the years. While the business is established, there is potential to maximize revenue by increasing the number of members, who are the company’s primary source of income. Cyclistic collects detailed data on both casual users and members, including their activity patterns on the service.

This project uses Excel to analyze bike-share data with the goal of uncovering the key differences between casual users and members. The insights gained aim to inform strategies that can boost membership adoption and revenue. 

## Data Description 

The source of the data examined in this project is Cyclistic; the analysis covers 12 months of data from December 2024 to December 2025. Combined, this dataset consists of over 1 million riders and 13 features describing each rider's trip. 

### Key Feature / Columns
- **ride_id**: A unique identifier for each ride
- **rideable_type**: Type of bike, classic or electric
- **started_at/ended_at**: The time and date of when the ride started and ended
- **member_casual**: Membership status of rider

## Methadology 
The 12 months of data were derived from monthly CSV files, which were imported to Power Query. The files were merged into a single dataset once the initial transformation of the organization was conducted using Power Query. While Power Query aided in the alignment and initial organization of data, there were still some discrepancies, as well as further preparation required to set up for the analysis. These steps consisted of the following:

- Removing the start_station_name, end_station_name, start_station_id, and end_station_id columns, there were many null values, and it served no purpose in what was intended with the data
- Scanned through the filter to remove outliers, ex. in the membership column, the only acceptable option is casual or member
- Removed any duplicate rows as well as blank rows
- Calculated the total duration of each ride by subtracting end_at from started_at
  - Coverted the duration value into total minutes
  - Then, using conditional formatting, created bins of time frames, ex. less than 10 min to enhance readability during analysis
- Extracted the day and month from the started_at column
- From the started_at column, created a column with the time, including just the hour of the day the trip started
  - Using conditional formatting created bins, ex. afternoon, so it is easier to understand than 15

## Analysis
During the analysis process, the primary tool used was pivot tables. By using pivot tables, over 1 million rows of data were efficiently organized into actionable insights. 

### Total Membership Split 
It was discovered that out of the million rider data, 25% of these riders were casual users, while the majority of 75% users were members. This reinforces the claim that the business is successful in its current efforts, but needs slight tweaks to convert the remaining 25% of users. 

### Weekly Trends 
When analyzing the line graph for the trends of users throughout the week, it was apparent that casual users have higher usage on the weekends, whereas members have higher usage during weekdays. This indicates that casual users are more likely to use this service for leisure, whereas members may use it as a means of commuting to work.

### Time of Day Trends
The analysis of this factor suggests that the majority of casual users use the bike service between hours of 12 pm and 4 pm, which is the afternoon. However, members use this service most between hours 5 pm to 8 pm, which is the evening. This insight reaffirms our former conclusion that most members use the bike-share for work commute, whereas casual users use it for leisure. 

### Ride Length Trends
The results of comparing the length of rides for each membership were similar, which shows that the distance travelled by these users wasn't an influencing factor of being a member. 

### Monthly Trends
While the results of both members' usage across a year were in consensus, there were some valuable insights. There is a spike in April that aligns with what one may assume as the weather is warmer; consequently, in colder months, there is lower usage as is inevitable. However, a discrepancy with this analysis is that the summer months are missing from the chart to confirm that summer had the highest usage. This issue was faced due to the maximum data capacity of Excel. A conclusion that could be derived using the analysis is that towards the warmer months, we saw an increase, which indicates that there could be an increase during summer and warmer months. 
 
## Reccomendations 

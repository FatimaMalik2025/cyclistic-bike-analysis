# Bike Share Analysis 

## Project Background
Launched in 2016, Cyclistic is a successful bike-sharing company that has expanded its services and marketing initiatives over the years. While the business is established, there is potential to maximize revenue by increasing the number of members, who are the company’s primary source of income. Cyclistic collects detailed data on both casual users and members, including their activity patterns on the service.

This project uses Excel to analyze bike-share data with the goal of uncovering the key differences between casual users and members. The insights gained aim to inform strategies that can boost membership adoption and revenue. 

## Data Description 

The data used for this project was provided by Cyclistic, and the analysis covers 12 months from December 2024 to December 2025. Combined, this dataset contains over 1 million riders, consisting of 13 features to describe each rider's trip. 

### Key Feature / Columns
- **ride_id**: A unique identifier for each ride
- **rideable_type**: Type of bike, classic or electric
- **started_at/ended_at**: The time and date of when the ride started and ended
- **member_casual**: Membership status of rider

## Methadology 
The 12 months of data were derived from monthly CSV files, which were imported to Power Query. The files were merged into a single data set, once the initial transformation of organization was conducted by Power Query. While Power Query aided in the alignment and initial organization of Power Query there were still some discrepencies, as well as further preperation required to set up for the analysis. These steps consisted of the following:

- Removing the start_station_name, end_station_name, start_station_id, and end_station_id columns there were many null values and it served no purpose in what was intended with the data
- Scanned through the filter to remove outliers ex. in the membership column the only acceptable option is casual or member
- Removed any duplicate rows as well as black rows
- Calculated the the total duration of each ride by subtracting end_at by started_at
  - Coverted the duration value into total min
  - Then using conditional fomatting created bins of time frames ex. less than 10 min to enhance readability during analysis
- Extracted the day and month from the started_at column
- From the started_at column created a column with the time including just the hour of the day the trip started
  - Using conditional formatting created bins ex. afternoon so it is easier to understand than 15

## Analysis

## Reccomendations 

# CitiBike-Dashboard
Tableau Dashboard - Data Analytics Course Module 18

# Task
In a hypothetical situation, as a lead analyst for the New York Citi Bike program, I will generate reports for city officials looking to publicize and improve the city program. I will be creating several dashboards and interactive map features.

# Methodology
## Data Selection and Cleaning

I selected the following files from the New York Citi Bike trip data for the year 2024:
 - 202401 (January)
 - 202404 (April)
 - 202407 (July)
 - 202410 (October)

The zip files for July and October were extremely large, containing between 5-6 CSV files each, resulting in millions of rows of data. I read in and concatenated the datasets into Pandas DataFrames. After removing null values, I created a new dataset for each month that sampled 5% of the original data, resulting in much more manageable file sizes while maintaining the integrity and precision of the data. Finally, I combined the cleaned individual month files into one ny_citibike_2024.csv.

## Dashboard: Growth Trends

![Growth_Trends](Images/growth_trends.jpg)

### - Ridership Growth by Bike Type
### - Total Trips per Week: 2024 Quarters

## Dashboard: User Trends

![User Trends](Images/user_trends_new.jpg)

### - Trip Duration: Member vs Casual User
### - Weekday Frequency: Member vs Casual User
### - User vs Bike Type
### - Peak Hours

## Dashboard: All Stations Map

![All stations map](Images/map.jpg)

## Dashboard: Top 10 Stations Map

![Growth_Trends](Images/top10_map.jpg)

## Results

The dashboard is available here: [Tableau](https://public.tableau.com/views/citibike_analysis_17392480645700/Story1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link).

## Analysis

![Analysis](Images/analysis.jpg)

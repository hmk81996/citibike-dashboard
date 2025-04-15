# Citi Bike Dashboard
An interactive **Tableau Dashboard** designed to provide insights related to ridership and membership, station usage, and seasonal trends.

# Problem
Since 2023, Citi Bike has collected, organized and made public data related to program use. However, there is no dashboard to provide city officials with regular, readable reports that support publicizing and improving the city program.

# Methodology
## Data Selection and Cleaning

I selected the following files from the New York Citi Bike trip data for the year 2024:
 - 202401 (January)
 - 202404 (April)
 - 202407 (July)
 - 202410 (October)

The zip files for July and October were extremely large, containing between 5-6 CSV files each, resulting in millions of rows of data. I read in and concatenated the datasets into Pandas DataFrames. After removing null values, I created a new dataset for each month that sampled 5% of the original data, resulting in much more manageable file sizes while maintaining the integrity and precision of the data. Finally, I combined the cleaned individual month files into one ny_citibike_2024.csv.

# Solution

These dashboards provide visualizations, reports, and recommendations.
- Growth Trends: Ridership Growth by Bike Type, Total Trips per Week: 2024 Quarters
- User Trends: Trip Duration, Weekday Frequency, User vs Bike Type, Peak Hours
- All Stations Map
- Top 10 Stations Map
 
![Growth_Trends](Images/growth_trends.jpg)

![User Trends](Images/user_trends_new.jpg)

![All stations map](Images/map.jpg)

![Growth_Trends](Images/top10_map.jpg)

The dashboard is available here: [Tableau](https://public.tableau.com/views/citibike_analysis_17392480645700/Story1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link).

# Analysis + Recommendations

![Analysis](Images/analysis.jpg)

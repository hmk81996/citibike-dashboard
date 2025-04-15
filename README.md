# Citi Bike Dashboard
An interactive **Tableau Dashboard** designed to provide insights related to ridership and membership, station usage, and seasonal trends.

# Problem
Since 2023, Citi Bike has collected, organized and made public data related to program use. However, there is no dashboard to provide city officials with regular, readable reports that support publicizing and improving the city program. Officials are seeking answers to the following questions:
- How did ridership change throughout the year?
- Who is riding? For how long? Where?
- Which start and end stations are most active?
- Based on the reports, what are recommendations for improviing the city program?

# Methodology
## Data Selection and Cleaning

I selected the following files from the New York Citi Bike trip data for the year 2024:
 - 202401 (January)
 - 202404 (April)
 - 202407 (July)
 - 202410 (October)

The zip files for July and October were extremely large, containing between 5-6 CSV files each, resulting in millions of rows of data. I read in and concatenated the datasets into Pandas DataFrames. After removing null values, I created a new dataset for each month that sampled 5% of the original data, resulting in much more manageable file sizes while maintaining the integrity and precision of the data. Finally, I combined the cleaned individual month files into one ny_citibike_2024.csv.

# Solution

These dashboards provide visualizations, reports, and recommendations and enable city officials to:
- 


# Key Features & Visualizations
- **Growth Trends**:
  - Line chart showing Ridership Growth by Bike Type
  - Bar Chart showing Total Trips per Week
- **Member vs. Casual User Trends**:
  - Bar charts showing Average Trip Duration, Weekday Frequency, User vs. Bike Type
  - Line Chart showing Peak Hours by Quarter
- **All Stations**: Interactive map showing most frequent start and end stations; user can toggle to a specific 2024 date.
- **Top 10 Stations**: Interactive map showing the Top 10 most frequent start and end stations; user can toggle to Start or End station.
  
![Growth_Trends](Images/growth_trends.jpg)

![User Trends](Images/user_trends_new.jpg)

![All stations map](Images/map.jpg)

![Growth_Trends](Images/top10_map.jpg)

The dashboard is available here: [Tableau](https://public.tableau.com/views/citibike_analysis_17392480645700/Story1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link).

# Analysis & Recommendations

![Analysis](Images/analysis.jpg)

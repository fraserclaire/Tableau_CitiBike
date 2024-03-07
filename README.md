# Tableau_CitiBike
Module 18 - Challenge
# Module 18 Challenge

## Goal: aggregate data in Citi Bike Trip History Logs to find two unexpected phenomena. Generate regular reports for city officials about the program.

## Questions to address:

- What are the top 10 stations for starting bike rides overall? Do all stations follow the same daily trend over time?
- What are the most popular stations for starting bike rides at different times of day (Dawn - 4AM to 10AM, Morning - 10AM to 4PM, Afternoon - 4PM to 10PM, Night - 10PM to 4AM)?
	- To inform prioritization/movement of bikes at these locations at those times


## Processing steps:

1. Download data files from [Citi Bike Trip Data]("https://citibikenyc.com/system-data")
	- JC station data files excluded, only downloaded data stored within the following:
		- "2023-citibike-tripdata.zip" , "2022-citibike-tripdata.zip"
	
2. Extracted .csv files from .zip folder to merge in Tableau
	- "202201-citibike-tripdata_1.csv", "202201-citibike-tripdata_#.csv", "202203-citibike-tripdata_#.csv"
	
3. Opened the files in Tableau
	- Opened the first file, then created a Union to merge all files	
	
## Tableau visualizations:

### Where are most bike rides starting at different times of the day? - Top Starting Station by Time 
https://public.tableau.com/app/profile/claire.fraser/viz/TopStartingStationbyTime/v2#1

### What are the most popular ride starting stations? - Top 10 Ride Start Stations
https://public.tableau.com/app/profile/claire.fraser/viz/OverallTopStartingStation/Overall-TopStartingStations-Jan2023?publish=yes
	
## Summary:

- In general, there are more stations with rides starting in March than January or February in both 2022 and 2023. This is likely due to the weather conditions being easier to ride a bike in during March, compared to January and February.
- Peak ride start times are ~8AM and ~6PM, which is likely due to the transit to and from work.

### Each month can be selected from the dropdown menu to conduct analyses on other months, such as below:

#### January 2023:

##### Where are most bike rides starting at different times of the day? - Top Starting Station by Time 
- The most popular stations to start bike rides in New York during the dawn and night hours (10PM-8AM) are located within the 10001 and 10018 zip codes. The radius of starting bike station locations during the morning and afternoon hours is larger, which may be due to these being peak times and potential need for riders to find available bikes at other nearby stops. This analysis can be done on a monthly or quarterly basis to identify which stations should be prioritized.

##### What are the most popular ride starting stations? - Top 10 Ride Start Stations
- Station 6140.05 had approximately 2-3K more starting rides than the other top 10 starting stations, however the most popular station at 8AM was station 6822.09 with about 200 more starting rides. The peak in starting rides at 8AM may be due to the station being in close proximity to many residences, as riders are likely starting a ride on their way to work. The station with the highest number of starting rides overall (Station 6140.05) peaked around 5-6PM, likely due to the station being nearby many businesses. The riders starting at this station may either be heading home from work or on their way home from running errands after work.

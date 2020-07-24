This folder contains files for: Analyze Bay Area Bike Share Data.

Bay\_Area\_Bike\_Share\_Analysis.ipynb - Main project file.

babs\_datacheck.py; babs\_visualizations.py - Supplemental scripts for checking
data wrangling, reporting of basic statistics, and creation of exploratory bar
charts and histograms.

Data is split among twelve other files, organized into three sets of four files
each. Prefixing each set is one of three datestamps, showing the end month for
each data collection period (201402, 201408, 201508). Suffixes for each file
indicate contents:

\*\_README.txt - Information about contents of data files.

\*\_station\_data.csv - Basic information about station locations and
capacities.

\*\_trip\_data.csv - Information about each trip taken using the bike share
system.

\*\_weather\_data.csv - Weather information by day for one station in each
city in the bike share program.

FILE LIST
1) 201402_status_data.csv – approx. 17 million records of status data (bike and dock availability)
2) 201402_station_data.csv – 69 records – station latitude, longitude, name, dockcount, installation date
3) 201402_trip_data.csv – approx. 144,000 records of individual trips
4) 201402_weather_data.csv – 920 records of daily weather by city

Files contain data from 8/29/13 (system launch) to 2/28/14.

1) STATUS DATA
FILE = "201402_status_data.csv"
-station_id: station ID number (use "201402_station_data.csv" to find corresponding station information)
-bikes_available: number of available bikes
-docks_available: number of available docks
-time: date and time, PST

2) STATION INFORMATION
FILE = "201402_station_data.csv"
-station_id: station ID number (corresponds to "station_id" in "201402_status_data.csv")
-name: name of station
-lat: latitude
-long: longitude
-dockcount: number of total docks at station
-landmark: city (San Francisco, Redwood City, Palo Alto, Mountain View, San Jose)
-installation: date that station was installed 

Note: Although stations were installed prior to 8/29/13 (system launch), no station was active until launch date. Therefore, to accurately capture station popularity, we recommend adjusting all pre-launch installation dates to 8/29/13.

3) TRIP DATA
FILE = "201402_trip_data.csv"
-Trip ID: numeric ID of bike trip
-Duration: time of trip in seconds
-Start Date: start date of trip with date and time, in PST
-Start Station: station name of start station
-Start Terminal: numeric reference for start station
-End Date: end date of trip with date and time, in PST
-End Station: station name for end station
-End Terminal: numeric reference for end station
-Bike #: ID of bike used
-Subscription Type: Subscriber = annual member; Customer = 24-hour or 3-day member
-Zip Code: Home zip code of user (only available for annual members)

4) WEATHER DATA
FILE = "201402_weather_data.csv"
Daily weather information per service area. Weather is listed from north to south (San Francisco, Redwood City, Palo Alto, Mountain View, San Jose).
	
-Max_Visibility_Miles 	Note-No local Mountain View historical visibility data- reported from Palo Alto station	
-Mean_Visibility_Miles 	Note-No local Mountain View historical visibility data- reported from Palo Alto station	
-Min_Visibility_Miles 	 Note-No local Mountain View historical visibility data- reported from Palo Alto station		
-Precipitation_In 	"numeric, in form x.xx but alpha ""T""= trace when amount less than .01 inch"	
-Cloud_Cover 	"scale of 0-8, 0=clear"	
-Events	"text field - entries: rain, fog, thunderstorm"	
-zip code: 94107=San Francisco, 94063=Redwood City, 94301=Palo Alto, 94041=Mountain View, 95113= San Jose"	
© 2020 GitHub, Inc.
Terms

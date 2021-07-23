# Analyzing MTA Stations: Foot traffic and Recovery Rate
Matthew Kwee

### Abstract
In this project, I analyzed MTA data scraped from the MTA's official website in order to find high-traffic stations that had quickly recovered from COVID-19 lockdowns. After calculating monthly ridership per station, I sent multiple requests to a Google Maps API to collect each station's geographical location, which I used to plot stations on a map of New York City.


### Design



### Data
There are 27.3 million turnstile datapoints for the period I analyzed (Jan.2019-Jul.2021). Each datapoint has 11 features, and 7 are categorical. Once I calculated daily ridership for each turnstile, I was able to group all the data into monthly ridership for each station.

### Algorithms
1. Calculating daily entries and exits for each turnstile.
2. Combining all turnstiles in each station to calculate station's daily traffic, then combining each day in each station to get monthly traffic.
3. Using Google Maps API to obtain geographic coordinates for each station, and using this data to plot stations on a map.


### Tools
SQLAlchemy for pulling initial data into Pandas
Pandas for data manipulation
Matplotlib for visualizing data
Google Maps Geocoding API to get stations' geographical coordinates




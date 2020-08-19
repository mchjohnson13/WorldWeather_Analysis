# WorldWeather_Analysis
## Task
Collect and analyze weather data accross cities worldwide
  
## Purpose
PlanMyTrip will use data to recomend ideal hotels based on clients' weather preferences.
  
## Method
Create a Pandas DataFrame with 500 or more of the world's unique cities and their weither data in real-time. This process will entail collecting, analyzing, and visualizing the data

### Data Analysis Process
1. Collect the Data
   * Use NumPy to generate more than 1500 random latitiudes and longitudes
   * Use citipy to list the nearest city latitiudes and longitudes
   * Use OpenWeather Map API to request the current weather data from each unique city in the list
   * Parse JSON data from API request
   * Collect from JSON file and add to DataFrame
     * City, Country, Date
     * Latitiude and longitude
     * Max temp
     * Humidity
     * Cloudiness
     * Wind Speed
2. Exploritory Analysis with Visualization
   * Create scatter plots
     * Latitude vs. temp
     * Latitude vs. humidity
     * Latitude vs. cloudiness
     * Latitude vs. wind speed
   * Determine correlations
   * Create a series of heat maps using Google Maps and Places API
3. Visualize Travel Data
   Create a heatmap with pop-up markers that can display information on specific cities based on customer travel preferences
     a. Filter Pandas DataFrame based on user inputs for min and max temp.
     b. Create heatmap for new DataFrame
     c. Find hotel from cities' coordinates and using Google Maps and Places API, and Search Nearby feature
     d. Store the name of the first hotel in the DataFrame
     e. Add pop-up markers to the heatmap that display information about the city, current max temp and a hotel in the city

# API-Challenge
In this project, I created analyzed current weather data from 600 cities around the world and identified suitable vacation locations based on weather criteria. WeatherPy analyzes compiles and analyzes the current weather. VacationPy identifies suitable vacation locations and plots them on a map. Below is a description of the included files and directories.
**Caution: running WeatherPy.ipynb will overwrite the existing output. If you would like to keep the existing output, copy outputs to a new file location.**
  
## Files and Directories
1. citylist.json
   - JSON file containing city, country, and coordinates for cities whose weather data is available at openweathermap.org
   - Columns:  
   -- 'id' : id for the city  
   -- 'name' : name of city  
   -- 'state' : state where the city is located (US only)  
   -- 'country' : two letter abbreviation for the country where the city is located  
   -- 'coord' : dictionary containing the latitude and longitude of the city. format = {'lon':longitude, 'lat':latitude}  
   - obtained from http://bulk.openweathermap.org/sample/ on 10/13/2020
2. VacationPy
   - Directory containing the vacation location analysis. 
   - VacationPy.ipynb:  
   -- Jupyter notebook that completes the analysis  
   -- **CAUTION:** This notebook is dependent on the output csv of WeatherPy.ipynb located at py-api-challenge/WeatherPy/outputs/weatherdata.csv  
   - outputs:  
   -- This directory containing a screenshot of the final map with the hotel markers and humidity heat map overlaid.
3. WeatherPy
    - Directory containing the weather data analysis.
    - WeatherPy.ipynb:  
    -- Jupyter notebook that assembles weatherdata.csv and analyzes current weather  
    -- Cities are selected as a sample of all cities available so results vary each time the notebook is run  
    - outputs:  
    -- Directory containing the results of analysis  
    -- LatCloud.png:  
    ---- Scatter plot of latitude vs cloudiness(%) in selected cities  
    -- LatHumid.png:  
    ---- Scatter plot of latitude vs humidity(%) in selected cities  
    -- LatTemp.png:  
    ----Scatter plot of latitude vs temperature(deg F) in selected cities  
    -- LatWind.png:  
    ---- Scatter plot of latitude vs wind speed(mph) in selected cities  
    -- weatherdata.csv:  
    ---- dataset of selected cities and their weather characteristics  
    ---- Columns (all values are current readings at time of request):  
    ------ 'name' : name of city  
    ------ 'country' : two letter abbreviation for country where city is located  
    ------ 'clouds' : cloudiness (%)  
    ------ 'humidity' : humidity (%)  
    ------ 'temp' : temperature (Fahrenheit)  
    ------ 'max_temp' : maximum currently observed temperature (Fahrenheit)  
    ------ 'wind_spd' : wind speed (mph)  
    ------ 'lat' : latitude (deg)  
    ------ 'lon' : longitude (deg)

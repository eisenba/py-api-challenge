# API-Challenge
In this project, I created analyzed current weather data from 600 cities around the world and identified suitable vacation locations based on weather criteria. WeatherPy analyzes compiles and analyzes the current weather. VacationPy identifies suitable vacation locations and plots them on a map. Below is a list of the values returned and a list of the included files.
**Caution: running WeatherPy.ipynb will overwrite the existing output. If you would like to keep the existing output, copy outputs to a new file location.**
  
## Files and Directories
1. citylist.json
   * JSON file containing city, country, and coordinates for cities whose weather data is available at openweathermap.org
   * Columns:
    *'id': id for the city
   -- 'name': name of city
   -- 'state': state where the city is located (US only)
   -- 'country': two letter abbreviation for the country where the city is located
   -- 'coord': dictionary containing the latitude and longitude of the city. format = {'lon':<longitude>, 'lat':<latitude>}
   - obtained from http://bulk.openweathermap.org/sample/ on 10/13/2020
2. VacationPy
   - Directory contains the input csv file. 
   - input csv must be in this directory and must be named 02-Homework_03-Python_Instructions_PyBank_Resources_budget_data.csv
3. WeatherPy
    - Directory contains the output txt file.
    - PyBank_output.txt contains the output values. This file is overwritten during each run of main.py

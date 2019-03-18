Weather and Air Quality (AirVisual)
===================================

Provides numeric information about weather and air quality:

* Temperature
* Atmospheric Pressure
* Wind speed
* Humidity
* Weather type
* Air Quality

The system uses IP geo-localization to find the nearest weather station of the monitoring agent.

Leverages [AirVisual](airvisual.com) through their REST API.

Required Macros:
----------------
* `%{APIKEY}`: API Key obtained from https://www.airvisual.com/dashboard/api

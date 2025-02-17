Weather and Air Quality (AirVisual)
===================================

[![Download](https://img.shields.io/badge/Download-Click%20Here-blue)](https://raw.githubusercontent.com/sentrysoftware/studioX-templates/refs/heads/master/templates/airVisual/airVisual.cfg) [![Need Support?](https://img.shields.io/badge/Need%20Support%3F-Click%20Here-blue)](https://www.sentrysoftware.com/bmc/about#section-contact)

> No support is provided for this template unless purchased. Refer to [Support for Monitoring Studio X Templates](../../support.md) for more details.

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

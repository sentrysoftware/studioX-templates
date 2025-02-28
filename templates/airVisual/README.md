Weather and Air Quality (AirVisual)
===================================

[![Static Badge](https://img.shields.io/badge/DOWNLOAD-.cfg-blue?style=for-the-badge&color=B071DC)](https://github.com/sentrysoftware/studioX-templates/raw/refs/heads/master/templates/airVisual/airVisual.cfg) [![Static Badge](https://img.shields.io/badge/-GET_SUPPORT-blue?style=for-the-badge&color=004577)](https://www.sentrysoftware.com/about/index.html#section-contact)

> [!CAUTION]
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

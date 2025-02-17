Weather and Air Quality (AirVisual)
===================================

![Static Badge](https://img.shields.io/badge/Download%20-%20Click%20Here-blue?link=https%3A%2F%2Fraw.githubusercontent.com%2Fsentrysoftware%2FstudioX-templates%2Frefs%2Fheads%2Fmaster%2Ftemplates%2FairVisual%2FairVisual.cfg)      ![Static Badge](https://img.shields.io/badge/Need%20Support%3F%20-%20Click%20Here-blue?link=https%3A%2F%2Fwww.sentrysoftware.com%2Fbmc%2Fabout%23section-contact)

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

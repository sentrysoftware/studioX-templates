Prometheus Exporter
===================

Requires Monitoring Studio X v10.3 or Higher.

Consumes data exposed by a Prometheus exporter.

The data is sorted by metric types:
* Bytes (converted to MB to try and stay below the highest acceptable value for a PATROL parameter)
* Fractions
* Hertz / MHz
* Seconds
* Other metrics

Feel free to add, remove, modify the Dynamic Instances representing the metric types.
Add thresholds when appropriate.

Import the .cfg file to add it to list of Templates.
Set the %{ENDPOINT} and %{PORT} macros with the appropriate values.

For more information about the Prometheus Exporter Template, refer to [Consuming Prometheus Metrics in Monitoring Studio X](https://www.sentrysoftware.com/support/user-documentation.html).

Prometheus Exporter
===================

[![Static Badge](https://img.shields.io/badge/DOWNLOAD-.cfg-blue?style=for-the-badge&color=B071DC)](https://github.com/sentrysoftware/studioX-templates/raw/refs/heads/master/templates/prometheus-exporter/prometheusExporterTemplate.cfg) [![Static Badge](https://img.shields.io/badge/-GET_SUPPORT-blue?style=for-the-badge&color=004577)](https://www.sentrysoftware.com/about/index.html#section-contact)

> [!CAUTION]
> No support is provided for this template unless purchased. Refer to [Support for Monitoring Studio X Templates](../../support.md) for more details.

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

For more information about the Prometheus Exporter Template, refer to [Consuming Prometheus Metrics in Monitoring Studio X](https://www.sentrysoftware.com/library/swsyx/prometheus/consuming-prometheus-metrics-in-patrol.html).

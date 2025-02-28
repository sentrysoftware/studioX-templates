F5 BigIP Monitoring
===================

[![Static Badge](https://img.shields.io/badge/DOWNLOAD-.cfg-blue?style=for-the-badge&color=B071DC)](https://github.com/sentrysoftware/studioX-templates/raw/refs/heads/master/templates/f5-BigIP/f5BigIp.cfg) [![Static Badge](https://img.shields.io/badge/-GET_SUPPORT-blue?style=for-the-badge&color=004577)](https://www.sentrysoftware.com/about/index.html#section-contact)

> [!CAUTION]
> No support is provided for this template unless purchased. Refer to [Support for Monitoring Studio X Templates](../../support.md) for more details.

Provides monitoring of the F5 Big IP appliance:

* Device Hardware Health and Status.
* Performance of Packet Velocity Acceleration engines, Overall System, Traffic Management Modules, System Software Volumes and Interfaces.

The template uses the embedded SNMP Agent on the appliance.

* Add the F5 BigIP appliance under the hosts tab and define the system type as `other`.
* Provide appropriate SNMP v2c community string and port number.

Note: If you see the value as N/A for metrics collected in `bytes`, consider re-scaling the value to convert into `kbytes`.

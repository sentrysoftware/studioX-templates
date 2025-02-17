Nutanix Appliance Monitoring - SNMP
===================================

[![Static Badge](https://img.shields.io/badge/DOWNLOAD-.cfg-blue?style=for-the-badge&color=B071DC)](https://github.com/sentrysoftware/studioX-templates/raw/refs/heads/master/templates/nutanix/nutanix-SNMP.cfg) [![Static Badge](https://img.shields.io/badge/-_GET_SUPPORT-blue?style=for-the-badge&color=004577)](https://www.sentrysoftware.com/about/index.html#section-contact)

> [!CAUTION]
> No support is provided for this template unless purchased. Refer to [Support for Monitoring Studio X Templates](../../support.md) for more details.

Monitors the Nutanix Appliance Cluster.

* Cluster Status, Storage and IOPS
* Container Information
* Controller Information
* Disks
* Hypervisor
* Storage Pool
* Virtual Machine

The template uses the embedded SNMP Agent on the Nutanix appliance.

* Add the Nutanix appliance Cluster under the hosts tab and define the system type as `other`.
* Provide appropriate SNMP community string or credentials and port number.

MONGO DB Monitoring
===================

[![Static Badge](https://img.shields.io/badge/DOWNLOAD-.cfg-blue?style=for-the-badge&color=B071DC)](https://github.com/sentrysoftware/studioX-templates/raw/refs/heads/master/templates/mongoDB/mongodb.cfg) [![Static Badge](https://img.shields.io/badge/-GET_SUPPORT-blue?style=for-the-badge&color=004577)](https://www.sentrysoftware.com/about/index.html#section-contact)

> [!CAUTION]
> No support is provided for this template unless purchased. Refer to [Support for Monitoring Studio X Templates](../../support.md) for more details.

Monitors the Mongo Data base through SNMP.

* Asserts
* Background Flushing
* Connections
* Cursors
* Data Directory
* File system
* Global Operation Counts
* Journal
* Memory
* Log File
* Network
* Process
* Replication Operation Counts
* System
* Current Queue
* Active Clients
* Document Metrics
* GetLastError
* Replication

Import the cfg and set the "Applies to Host System Type" to the appropriate OS type depending on the OS running on the server where the Mongo DB is installed.
Add the host and provide appropriate SNMP community string.
Set the %{DATA_DIR} and %{MONGO_LOGFILE} macros with appropriate values.

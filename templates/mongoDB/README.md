MONGO DB Monitoring
===================

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

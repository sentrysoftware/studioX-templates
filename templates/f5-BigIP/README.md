F5 BigIP Monitoring
===================

Provides monitoring of the F5 Big IP appliance:

* Device Hardware Health and Status.
* Performance of Packet Velocity Acceleration engines, Overall System, Traffic Management Modules, System Software Volumes and Interfaces.

The template uses the embedded SNMP Agent on the appliance.

* Add the F5 BigIP appliance under the hosts tab and define the system type as `other`.
* Provide appropriate SNMP v2c community string and port number.

Note: If you see the value as N/A for metrics collected in `bytes`, consider re-scaling the value to convert into `kbytes`.

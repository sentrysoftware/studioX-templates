Microsoft IIS Server Monitoring
====================================

[![Static Badge](https://img.shields.io/badge/DOWNLOAD-.cfg-blue?style=for-the-badge&color=B071DC)](https://github.com/sentrysoftware/studioX-templates/raw/refs/heads/master/templates/microsoft-IIS/microsoftIIS.cfg) [![Static Badge](https://img.shields.io/badge/-_GET_SUPPORT-blue?style=for-the-badge&color=004577)](https://www.sentrysoftware.com/about/index.html#section-contact)

> [!CAUTION]
> No support is provided for this template unless purchased. Refer to [Support for Monitoring Studio X Templates](../../support.md) for more details.

Provides monitoring of Microsoft IIS Server:

* Performance Metrics - User can add more Windows Performance counters related to IIS for Monitoring.
* Application Pools - Monitors Status
* Websites - Monitors Status

Pre-requisites

* Powershell version 5.1 or above installed on monitored host
* Module IISAdministration installed on monitored host
* Powershell Execution Policy needs to be set to allow the scripts to be run, typically `RemoteSigned`.

Using the Template

* Add the IIS server under the hosts tab and define the system type as `Windows`.
* Provide appropriate username and password for System Credentials to access the server.
* Activate the Microsoft IIS Server Template for the newly added host and "Save".

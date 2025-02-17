Microsoft Project Server Monitoring
====================================================

[![Static Badge](https://img.shields.io/badge/DOWNLOAD-.cfg-blue?style=for-the-badge&color=B071DC)](https://github.com/sentrysoftware/studioX-templates/raw/refs/heads/master/templates/microsoft-Project-Server/projectserver.cfg) [![Static Badge](https://img.shields.io/badge/-_GET_SUPPORT-blue?style=for-the-badge&color=004577)](https://www.sentrysoftware.com/about/index.html#section-contact)

> [!CAUTION]
> No support is provided for this template unless purchased. Refer to [Support for Monitoring Studio X Templates](../../support.md) for more details.

Provides monitoring of Microsoft Project Server 2013/2016/2019:

Microsoft Project Server Event Logs - User can add more Event Logs to monitor
Microsoft Project Server - User can add more Windows Performance counters related to SharePoint for Monitoring.
Windows Project Server Services
Microsoft Project Server cmdlets - Database size and health check parsing

Using the Template

- Add the Microsoft Project Server server under the hosts tab and define the system type as Windows.
- Provide appropriate username and password for System Credentials to access the server.
- Also provide Site Admin Credentials if the user name to access the Admin Site is different from the System Credentials.
- The services' names will need to be adjusted depending on the version (default: 2016, eg: ProjectCalcService16).
- As Microsoft Project Server is dependant on Microsoft SharePoint, it is recommended to use both templates concurrently.

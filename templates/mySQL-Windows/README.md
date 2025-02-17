MySQL Database Monitoring
=========================

[![Static Badge](https://img.shields.io/badge/DOWNLOAD-.cfg-blue?style=for-the-badge&color=B071DC)](https://github.com/sentrysoftware/studioX-templates/raw/refs/heads/master/templates/mySQL-Windows/MySQLWindows.cfg) [![Static Badge](https://img.shields.io/badge/-GET_SUPPORT-blue?style=for-the-badge&color=004577)](https://www.sentrysoftware.com/about/index.html#section-contact)

> [!CAUTION]
> No support is provided for this template unless purchased. Refer to [Support for Monitoring Studio X Templates](../../support.md) for more details.

Monitors the MySQL Database installed on a Windows server.

Provides monitoring of:

* Logs
* Data Directory
* Performance metrics of Innodb, Tables and Files, Performance Schema etc.
* mysqld process Metrics
* file IOPS
* Mutex waits
* Running Processes
* Replication Slave status

In addition, you can add SQL queries and process the results using the "Analysis" feature.

* Import the cfg and activate it on the Host where the MySQL Database is installed.
* Set the System Credentials to logon to the system and execute the mysqladmin binary.
* Set the Credentials "mysqlroot" to access the Database

Set the following macros with appropriate values:
%{MYSQL_PATH} - Path to the mysqladmin binary
%{MYSQL_USER}  - Username as in "mysqlroot"
%{MYSQL_PASSWORD} - Password as in "mysqlroot"
%{DATA_DIR} - Data directory of the MySQL Database
%{MYSQL_LOG} - Log file location

On the Host Settings, provide appropriate Database name and port number under MySQL Database Connection Settings.

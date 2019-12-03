MySQL Database Monitoring
=========================

Monitors the MySQL Database installed on a Linux server.

Provides monitoring of:
* Logs
* Data Directory
* Performance metrics of Innodb, Tables and Files, Performance Schema etc.
* mysqld process Metrics
* file IOPS

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

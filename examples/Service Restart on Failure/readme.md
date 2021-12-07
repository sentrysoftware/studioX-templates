<strong>Service Restart on Failure</strong>
====================================================
This template shows how to setup monitoring and an alert action in order to restart a service should it stop. In this scenario, we have a service monitor set to alert us should it go down, and we have a command monitor, which is set to only run manually. In our service monitor configuration, we configured an alarm action for when the service is "stopped", which will launch the command line monitor, prompting the service to start.

<strong>Windows Service Monitor - Service: SNMP Trap</strong>

In this monitor, we are simply selecting a service to monitor. We can set different status based on what should be the expected status of the service. We have then set an Alarm that will automatically launch our other monitor, attempting to restart the service.

Sample output:
```
Service Name: SNMPTRAP
Description: SNMP Trap;
State: Running (OK)
Account: NT AUTHORITY\LocalService
Exit Code: 0
```
<strong>Command Line Monitor - Service Restart Command</strong>

Command run on host:
```bat
net start SNMPTRAP
```
In this monitor, we are simply launching the command that will start our problematic service. Important note here is that we set this command to only run manually (or in our case, when called as an alert action). This is to avoid the host to attempt to truncate the logs every two minutes (default collection interval).

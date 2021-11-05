<strong>Automatic Log Truncation</strong>
====================================================
This template shows how to monitor a partition size and truncate the associated log to free up space. This specific example was done for EMC VNXe hosts where monitoring of the system caused the audit logs to swell to problematic sizes.

<strong>Command Line Monitor - Command Log Size Verification</strong>

Command ran on host:
df -h /EMC/backend/log_shared

In this monitor, we are simply launching the command that will gather the size of the partition where the log is stored. This command will likely be different based on the platform against which it is used or even based on system configuration.

Sample output:
Filesystem                    Size  Used  Avail   Use%  Mounted on
/EMC/backend/log_shared       251G  2.2G  236G    1%    /EMC

<strong>Numeric Extraction - Log Size Numeric Extraction</strong>

This monitor is where we will extract the partition value and set whichever alerts we may want. Since we know the value is followed by a "%", we opted to use "Before this String: %" to locate the relevant value. In the alert options, we set an information alert threshold at partition usage of 50% and an alert action, which calls a separate command line monitor which we will review below.

We then also added an alarm alert at a threshold of 60% usage, so that we receive an alert if for some reason, the log truncation does not clear space, meaning we will need the system admin to review the situation.

<strong>Command Line Monitor - Log Truncate</strong>

Command ran on host:
psql -U c4 c4LoggingDatabase -c 'truncate "CST_LogRecord" cascade'

In this monitor, we are simply launching the command that will truncate our problematic log file. This command will almost certainly be different based on the platform against which it is used or even based on system configuration. Important note here is that we set this command to only run manually (or in our case, when called as an alert action). This is to avoid the host to attempt to truncate the logs every two minutes (default collection interval).

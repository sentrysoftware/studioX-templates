<strong>All Performance Counter Instances Using Command Line</strong>
====================================================
This template shows how to monitor all Performance Counter Instances concurrently while using only a single command line monitor. In this example, we use this template to gather "% User Time" counter from all logical cores on the host. This could be ideal when using a template with a large or unknown number of cores, as this will create an instance for each core present as well as the _total instance.

<strong>Command Line Monitor - Command Gathering All Desired Performance Counter Instances</strong>

Command ran on host:
wmic path Win32_PerfFormattedData_PerfOS_Processor get Name,PercentUserTime /value /format:CSV

In this monitor, we are simply launching the command that will gather all the instances using the wmic command for windows. We added /value and /format:CSV for formatting reasons. Each value will be listed on a separate line and it will be formatted as a CSV, separated by commas. This will come in handy in the next step. Note that this will require valid System Credentials.

The first column will be your hostname, the second will be the instance name and the third one will be the actual value we want monitored: % User Time.

Sample output:

Node,Name,PercentUserTime
ExampleHostname,0,0
ExampleHostname,1,12
ExampleHostname,2,6
ExampleHostname,3,6
ExampleHostname,_Total,11

<strong>Dynamic Instances - Performance Counter Instances</strong>

In this monitor, we use dynamic instances to create one MSX instance per Performance Counter instance. This way, we will be able to separate all of the instances, so that each can be monitored independently. By specifying the CSV format earlier, we can now set our Column Separators as ",". Since our processor name will be different for each instance, it makes it the ideal column to use for the Dynamic Instance Internal ID and Dynamic Instance Display Name. We also used the option "Keep Lines Matching" and set it to [0-9], meaning only lines with numeric values will be kept, essentially ignoring empty lines as well as the header.

<strong>Numeric Extraction - Percent User Time</strong>

This monitor is where we will extract the PercentUserTime value and set whichever alerts we may want. Similarly as the above monitor, we need to set the Column Separator to "," and then specify the value as being in column number 3. In this example, we set the warning threshold at 95% or above and the alarm threshold at 100%.

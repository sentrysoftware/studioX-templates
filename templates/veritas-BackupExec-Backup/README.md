## Veritas Backup Exec (formerly Symantec Backup Exec)

This is a Monitoring Studio X template for monitoring Veritas Backup Exec v20+ on Windows platforms.
It monitors:
- Agent Servers
- Alerts
- Jobs (completed and active)
- Services
- Storage Device Servers
- Storage Devices

The template uses the Backup Exec PowerShell module *BEMCLI* to execute commands on the Backup Exec Servers. Ensure that the user account used for monitoring has access to execute the module.

## Configuring through Monitoring Studio X Web UI

* Add the Backup Exec Server host under the *Monitored Hosts* tab and define the system type as *Microsoft Windows*.
* Provide appropriate user credentials to access the server.
* Activate the *VERITAS BACKUP EXEC* template and click on Create.

## Configuring through TrueSight/Helix CMA

Once the template is imported into a TrueSight/Helix CMA policy for Monitoring Studio X (Configuration Variables), you need to:
- add the Backup Exec servers with appropriate *System Credentials* that allow connecting to the server and run Backup Exec BEMCLI
- associate the template (*backupExec*)
- (optional) change the default macros by adding them to the *Required Macros*

## Required Macros

The templates use following required macros. If you prefer to leave as default, do not add them to the *Required Macros* in the *Associated Templates* in the TrueSight CMA policy.
- **JOB_HOURS**: Number of hours completed jobs are monitored for. Default: 48 hours

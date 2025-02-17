Windows Scheduled Task
======================

[![Static Badge](https://img.shields.io/badge/DOWNLOAD-.cfg-blue?style=for-the-badge&color=B071DC)](https://github.com/sentrysoftware/studioX-templates/raw/refs/heads/master/templates/win-schtasks/win-schtasks.cfg) [![Static Badge](https://img.shields.io/badge/-_GET_SUPPORT-blue?style=for-the-badge&color=004577)](https://www.sentrysoftware.com/about/index.html#section-contact)

> [!CAUTION]
> No support is provided for this template unless purchased. Refer to [Support for Monitoring Studio X Templates](../../support.md) for more details.

Monitors Windows' Scheduled Tasks:

* Status of the Schedule Service
* Number currently running tasks
* For each active scheduled task:
    * Status (Running or not)
    * Last execution result (OK or not)
    * Time since last execution (in hours)

Use the `EXCLUDE_TASKS_REGEX` macro to specify a regular expression to exclude specific tasks. Example: `BrokerInfrastructure\|MemoryCheck`

> Note: You need to use PSL's *grep()* syntax. `exprA\|exprB` means `exprA` **OR** `exprB`.

**IMPORTANT: Requires Monitoring Studio X 10.3**

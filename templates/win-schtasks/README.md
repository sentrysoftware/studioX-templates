Windows Scheduled Task
======================

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

Microsoft Office 365 Monitoring
====================================================

[![Static Badge](https://img.shields.io/badge/DOWNLOAD-.cfg-blue?style=for-the-badge&color=B071DC)](https://github.com/sentrysoftware/studioX-templates/raw/refs/heads/master/templates/microsoft-Office365-Powershell/office365Powershell.cfg) [![Static Badge](https://img.shields.io/badge/-GET_SUPPORT-blue?style=for-the-badge&color=004577)](https://www.sentrysoftware.com/about/index.html#section-contact)

> [!CAUTION]
> No support is provided for this template unless purchased. Refer to [Support for Monitoring Studio X Templates](../../support.md) for more details.

Provides monitoring of Office 365 via Powershell cmdlets:

Subscriptions - Total subscriptions, Used subscriptions and warning subscriptions
Groups - Validation Status, Directory Sync Provisioning Errors, Errors
Services - Service Status
Mailbox Quotas - Lists and creates warnings/alarms mailboxes that have reached either "IssueWarning" or "ProhibitSend" thresholds.

Prerequisites to be installed on the Patrol Agent:
PowerShell 5.0 or higher
.NET 4.7.1 or higher
Powershell modules: ExchangeOnlineManagement, MSOnline

Steps:

- When assigning the template to the hosts, the Office 365 Credentials must be provided for the cmdlets to function.
- The proper Execution Policies must be set for the user running the powershell cmdlets. See https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-7.1 for more information.
- The office365Powershell:subscriptions:subscriptionsBySKU:licensesUsed monitor thresholds need to be configured manually at this time.

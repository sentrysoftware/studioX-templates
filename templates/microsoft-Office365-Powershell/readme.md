<strong>Microsoft Office 365 Monitoring</strong>
====================================================
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
- The office365Powershell:subscriptions:subscriptionsBySKU:licensesUsed monitor thresholds need to be configured manually at this time.
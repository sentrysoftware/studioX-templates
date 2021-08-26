Monitoring Oracle Private Cloud Appliance
=========================================
Monitoring the overall health of the components in the Private Cloud Appliance using the pca-admin cli.

* Compute Nodes
* Management Nodes
* Network Ports
* Tasks
* Tenant Groups
* Uplink Ports

The ZFS Storage of the PCA can be monitored using the Hardware Sentry KM: https://www.sentrysoftware.com/library/hc/24/MS_HW_SunZFSStorageAppliance.html

The **Compute Nodes** and the **Management Nodes** can be monitored using the Hardware Sentry KM through the ILOMs: https://www.sentrysoftware.com/library/hc/24/MS_HW_SunILOMSSH.html

Set Up
------

* Add the Oracle PCA under the **Hosts** tab and choose the **System Type** as **Linux**.

* Provide the System Credentials to execute the pca-admin command on the PCA.

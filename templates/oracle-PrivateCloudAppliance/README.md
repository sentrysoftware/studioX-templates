Monitoring Oracle Private Cloud Appliance
=========================================

[![Static Badge](https://img.shields.io/badge/DOWNLOAD-.cfg-blue?style=for-the-badge&color=B071DC)](https://github.com/sentrysoftware/studioX-templates/raw/refs/heads/master/templates/oracle-PrivateCloudAppliance/oraclePrivateCloudAppliance.cfg) [![Static Badge](https://img.shields.io/badge/-_GET_SUPPORT-blue?style=for-the-badge&color=004577)](https://www.sentrysoftware.com/about/index.html#section-contact)

> [!CAUTION]
> No support is provided for this template unless purchased. Refer to [Support for Monitoring Studio X Templates](../../support.md) for more details.

Monitoring the overall health of the components in the Private Cloud Appliance using the pca-admin cli.

* Compute Nodes
* Management Nodes
* Network Ports
* Tasks
* Tenant Groups
* Uplink Ports

The ZFS Storage of the PCA can be monitored using the [Hardware Sentry KM](https://www.sentrysoftware.com/docs/hardware-connectors/24/MS_HW_SunZFSStorageAppliance.html).

The **Compute Nodes** and the **Management Nodes** can be monitored using the [Hardware Sentry KM through the ILOMs](https://www.sentrysoftware.com/docs/hardware-connectors/24/MS_HW_SunILOMSSH.html)

Set Up
------

* Add the Oracle PCA under the **Hosts** tab and choose the **System Type** as **Linux**.

* Provide the System Credentials to execute the pca-admin command on the PCA.

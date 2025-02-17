Dell EMC VIPR Controller Monitoring
===================================

[![Static Badge](https://img.shields.io/badge/DOWNLOAD-.cfg-blue?style=for-the-badge&color=B071DC)](https://github.com/sentrysoftware/studioX-templates/raw/refs/heads/master/templates/emc-VIPRController/dellEmcViprController.cfg) [![Static Badge](https://img.shields.io/badge/-_GET_SUPPORT-blue?style=for-the-badge&color=004577)](https://www.sentrysoftware.com/about/index.html#section-contact)

> [!CAUTION]
> No support is provided for this template unless purchased. Refer to [Support for Monitoring Studio X Templates](../../support.md) for more details.

Provides monitoring of the Dell EMC VIPR Controller appliance:

* Node Diagnostics
* DB Consistency Status
* Health
* IPSec Status
* Site Status
* Performance Statistics
* Storage Capacity Metrics

The template uses the VIPR Controller's REST API.

* Add the VIPR Controller host under the hosts tab and define the system type as `Other`.
* Provide appropriate username and password to access the REST API as system credentials.
* Specify the port number while activating the template if it is other than 4443

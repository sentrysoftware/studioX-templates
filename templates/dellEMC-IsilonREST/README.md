DELL EMC ISILON Monitoring
==========================

[![Static Badge](https://img.shields.io/badge/DOWNLOAD-.cfg-blue?style=for-the-badge&color=B071DC)](https://github.com/sentrysoftware/studioX-templates/raw/refs/heads/master/templates/dellEMC-IsilonREST/dellEmcIsilonRest.cfg) [![Static Badge](https://img.shields.io/badge/-GET_SUPPORT-blue?style=for-the-badge&color=004577)](https://www.sentrysoftware.com/about/index.html#section-contact)

> [!CAUTION]
> No support is provided for this template unless purchased. Refer to [Support for Monitoring Studio X Templates](../../support.md) for more details.

Provides monitoring of the Dell EMC Isilon One FS Cluster:

* Client Statistics
* Deduplication Jobs Summary
* Drive Statistics
* File System Statistics
* Node Resources
* Nodepools
* OneFS Feature Licenses
* Protocol Summary
* Storagepools
* System Statistics
* Workload Statistics

In addition to the above configured metrics, you can retrieve the metrics for other licensed components and protocols.

The template uses the Dell EMC Isilon REST API.

* Add the Isilon Cluster host under the hosts tab and define the system type as `Other`.
* Provide appropriate username and password to access the REST API as system credentials.

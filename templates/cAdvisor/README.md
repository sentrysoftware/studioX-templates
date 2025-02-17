Docker Monitoring using cAdvisor
================================

[![Static Badge](https://img.shields.io/badge/DOWNLOAD-.cfg-blue?style=for-the-badge&color=B071DC)](https://github.com/sentrysoftware/studioX-templates/raw/refs/heads/master/templates/cAdvisor/cadvisor.cfg) [![Static Badge](https://img.shields.io/badge/-GET_SUPPORT-blue?style=for-the-badge&color=004577)](https://www.sentrysoftware.com/about/index.html#section-contact)

> [!CAUTION]
> No support is provided for this template unless purchased. Refer to [Support for Monitoring Studio X Templates](../../support.md) for more details.

This template provides monitoring of the docker containers and file systems using cAdvisor (https://github.com/google/cadvisor).

* File System Statistics
* Container statistics

The template uses the cAdvisor REST API.

* Add the Docker host under the hosts tab and define the system type as `Other`.
* Specify the port on which the cAdvisor exposes metrics under the PORT macros.

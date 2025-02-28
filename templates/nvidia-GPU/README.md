Nvidia GPU Monitoring
=====================

[![Static Badge](https://img.shields.io/badge/DOWNLOAD-.cfg-blue?style=for-the-badge&color=B071DC)](https://github.com/sentrysoftware/studioX-templates/raw/refs/heads/master/templates/nvidia-GPU/nvidiaGPU.cfg) [![Static Badge](https://img.shields.io/badge/-GET_SUPPORT-blue?style=for-the-badge&color=004577)](https://www.sentrysoftware.com/about/index.html#section-contact)

> [!CAUTION]
> No support is provided for this template unless purchased. Refer to [Support for Monitoring Studio X Templates](../../support.md) for more details.

Provides monitoring of the Nvidia graphics card:

* GPU Utilization
* GPU Temperature
* Memory
* Performance
* Power

The template uses the nvidia-smi cli utility installed on the server being monitored.

* Add the server with the GPU under the hosts tab and define the system type depending on the OS.
* Provide NVSMI_PATH value with the installation location of the nvidia-smi cli.

This is just a base and more commands can be configured to monitor additional metrics.

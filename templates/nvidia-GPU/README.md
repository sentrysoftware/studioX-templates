Nvidia GPU Monitoring
=====================

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

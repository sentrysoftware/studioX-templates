Docker Monitoring using cAdvisor
================================

This template provides monitoring of the docker containers and file systems using cAdvisor.

* File System Statistics
* Container statistics

The template uses the cAdvisor REST API.

* Add the Docker host under the hosts tab and define the system type as `Other`.
* Specify the port on which the cAdvisor exposes metrics under the PORT macros.

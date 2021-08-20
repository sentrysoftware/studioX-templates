Monitoring OpenStack
====================

Monitoring OpenStack environment using the OpenStack Command Line client.

* Images
* Ports
* Resource Limits
* Server List
* Resource Usage
* Volume List
* Zone Availability

The monitoring requires the OpenStack CLI to be installed on the (LINUX) server from where the Openstack is monitored. It can also be installed on the same server as the Patrol Agent and Monitoring Studio KM.

https://docs.openstack.org/newton/user-guide/common/cli-install-openstack-command-line-clients.html

Set up
------

* Create a user account for monitoring in the OpenStack.

* An OpenStack RC file is embedded in the template. Edit the below lines in the "openrc.sh" with appropriate values.
```bash
export OS_TENANT_ID=<TENANT_ID>
export OS_TENANT_NAME="<TENANT_NAME>"
export OS_USERNAME="<USER_NAME>"
```

* Add the host where the OpenStack CLI is installed and provide the system credentials to logon and execute the script.
* Activate the OpenStack Template and provide the password for the OpenStack user in the **OS_PASSWORD** macro field.

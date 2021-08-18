Monitoring Openstack
====================

Monitoring Openstack environment using the Openstack Command Line client.

* Images
* Ports
* Resource Limits
* Server List
* Resource Usage
* Volume List
* Zone Availability

The monitoring requires the Openstack CLI to be installed on the (LINUX) server where the Patrol Agent and the Monitoring Studio KM is installed.

https://docs.openstack.org/newton/user-guide/common/cli-install-openstack-command-line-clients.html

Set up
------

* Create a user account for monitoring.

* Set the Environment Variables: https://docs.openstack.org/newton/user-guide/common/cli-set-environment-variables-using-openstack-rc.html
 An Openstack RC file is embedded in the template. Edit the below lines in the embedded "openrc-demo-monitor.sh" with appropriate values.
```bash
export OS_TENANT_ID="<TENANT_ID>"
export OS_TENANT_NAME="<TENANT_NAME>"
export OS_USERNAME="<USER_NAME>"
```
* The password is required as a parameter. To workaround this prompt,set the password to the env variable $OS_PASSWORD_INPUT.
* Add the localhost with the credentials to execute the script and activate the Openstack Template.

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
 An Openstack RC file is embedded in the template. Copy the file under /root and edit the below lines "openrc-demo-monitor.sh" with appropriate values.
```bash
export OS_TENANT_ID="<TENANT_ID>"
export OS_TENANT_NAME="<TENANT_NAME>"
export OS_USERNAME="<USER_NAME>"
```
* The password is required as a parameter. To workaround this prompt,set the password comment the below lines
```bash
#read -sr OS_PASSWORD_INPUT
#export OS_PASSWORD=$OS_PASSWORD_INPUT
```
And provide the password directly
```bash
export OS_PASSWORD=t4467DqUuXkNFn4dWERChC7DGFH
```
Note: If you store the file in a different location other than /root please specify the same path in the **Command Line Execution** monitors.
```bash
. ./openrc-demo-monitor.sh ;openstack image list -f csv
```
to
```bash
 ./<FILEPATH>/openrc-demo-monitor.sh ;openstack image list -f csv
 ```
* Add the localhost with the credentials to execute the script and activate the Openstack Template.

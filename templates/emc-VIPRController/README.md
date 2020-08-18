Dell EMC VIPR Controller Monitoring
===================================

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

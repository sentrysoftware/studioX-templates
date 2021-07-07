<strong>Service Restart on Failure</strong>
====================================================
This template shows how to setup monitoring and an alert action in order to restart a service should it stop. In this scenario, we have a service monitor set to alert us should it go down, and we have a command monitor, which is set to only run manually. In our service monitor configuration, we configured an alarm action for when the service is "stopped", which will launch the command line monitor, prompting the service to start.

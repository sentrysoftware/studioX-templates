# Templates for Monitoring Studio X

This GitHub repository is a public collection of [Templates](//www.sentrysoftware.com/library/swsy10/hosts-templates.html) for [Monitoring Studio X](//www.sentrysoftware.com/products/km-monitoring-studio-x.asp), a monitoring solution developed by Sentry Software.

In a BMC TrueSight Operations Management environment, **Monitoring Studio X** will integrate natively as a regular KM for PATROL. But a single standalone PATROL Agent with Monitoring Studio KM will be enough to cover a small environment (less than 200 servers, typically).

&gt;&gt;&gt; [Check out the available Templates](//github.com/sentrysoftware/studioX-templates/tree/master/templates) &lt;&lt;&lt;

## Prerequisites

You will need:

* [Monitoring Studio X](//www.sentrysoftware.com/products/km-monitoring-studio-x.asp) (obviously)
* [BMC PATROL Agent](//docs.bmc.com/docs/PATROLAgent/11302/installing-828956013.html) (any version will do)

## How to use a template

Each template is in a separate sub-directory in [./templates](//github.com/sentrysoftware/studioX-templates/tree/master/templates).

Download the .cfg file and [import it in Monitoring Studio X](//www.sentrysoftware.com/library/swsy10/hosts-templates.html#Importing_a_Template).

In **Monitoring Studio X**, [create the Host](//www.sentrysoftware.com/library/swsy10/hosts-templates.html#Step_1_Defining_Hosts) you want to monitor with this *Template* and apply the *Template*.

Read carefully the associated **README.md** for instructions on the required configuration and technical prerequisites of the *Template*.

## Support and Maintenance

To be clear: these monitoring *Templates* may be provided by Sentry Software, but they are provided for free and no support or maintenance is guaranteed on these from [Sentry Support](//www.sentrysoftware.com/support/maintenance-policy.asp). Monitoring Studio X itself, however, is fully supported (if you are an entitled customer!).

Problems with these templates can be [raised on GitHub as an Issue](//github.com/sentrysoftware/studioX-templates/issues). If you find a problem with a *Template*, **DO NOT HESITATE** to fix it yourself and share with the community! See the [Contributing](CONTRIBUTING.md) section below! :-)

## Contributing

See [Contributing](CONTRIBUTING.md).

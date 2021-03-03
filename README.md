# Templates for Monitoring Studio X

This GitHub repository is a public collection of [Templates](//www.sentrysoftware.com/library/swsyx/hosts-templates.html) for [Monitoring Studio X](/www.sentrysoftware.com/products/km-monitoring-studio-x.html), a monitoring solution developed by Sentry Software.

In a BMC TrueSight Operations Management environment, **Monitoring Studio X** will integrate natively as a regular KM for PATROL. But a single standalone PATROL Agent with Monitoring Studio KM will be enough to cover a small environment (less than 200 servers, typically).

&gt;&gt;&gt; [Check out the available Templates](//github.com/sentrysoftware/studioX-templates/tree/master/templates) &lt;&lt;&lt;

## Prerequisites

You will need:

* [Monitoring Studio X](//www.sentrysoftware.com/products/km-monitoring-studio-x.asp) (obviously)
* [BMC PATROL Agent](//docs.bmc.com/docs/PATROLAgent/11302/installing-828956013.html) (any version will do)

## How to use a template

Each template is in a separate sub-directory in [./templates](//github.com/sentrysoftware/studioX-templates/tree/master/templates).

Download the .cfg file and [import it in Monitoring Studio X](//www.sentrysoftware.com/library/swsyx/hosts-templates.html#Importing_a_Template).

In **Monitoring Studio X**, [create the Host](//www.sentrysoftware.com/library/swsyx/hosts-templates.html#Step_1_Defining_Hosts) you want to monitor with this *Template* and apply the *Template*.

Read carefully the associated **README.md** for instructions on the required configuration and technical prerequisites of the *Template*.

## Support and Maintenance

To be clear: these monitoring *Templates* may be provided by Sentry Software, but they are provided for free and no support or maintenance is guaranteed on these from [Sentry Support](//www.sentrysoftware.com/support/maintenance-policy.asp). Monitoring Studio X itself, however, is fully supported (if you are an entitled customer!).

Problems with these templates can be [raised on GitHub as an Issue](//github.com/sentrysoftware/studioX-templates/issues). If you find a problem with a *Template*, **DO NOT HESITATE** to fix it yourself and share with the community! See the [Contributing](CONTRIBUTING.md) section below! :-)

## Contributing

Anyone is welcome to contribute in this library of monitoring templates for Monitoring Studio X!

### Instructions

1. Fork the [sentrysoftware.studioX-templates](//github.com/sentrysoftware/studioX-templates) repository. As a result, you will have your own **studioX-templates** repository in your GitHub account.
2. Create a branch from **master** with a proper name describing the addition or change you intend to bring
3. Commit your changes to this branch, and push this commit to your **studioX-templates** repository on GitHub. The changes must include:
    * A new sub-directory in **./templates** for a new *Template*
    * The template `.CFG` file, as exported from Monitoring Studio X
    * a short **README.md** that explains what the *Templates* monitors and how to configure it (the content of **README.md** is typically the same as the description field of the *Template* object)
4. Submit a *Pull Request* to the [master](//github.com/sentrysoftware/studioX-templates/tree/master) branch of the **sentrysoftware/studioX-templates** repository.

Thank you! :-)

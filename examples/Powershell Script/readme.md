<strong>Powershell</strong>
====================================================
This template shows how to use a powershell script within Monitoring Studio X, leveraging the Command Line monitor. The first example uses an embedded file, specified in the template configuration. The second option, features the same script, but on the host where this template is active.

For powershell scripts to run successfully, the execution policy needs to be set accordingly on the host where they will be run. See microsoft documentation for more information: https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-7.1

<strong>Command Line Monitor - Powershell Command Embedded File</strong>

Command run on host:
```bat
@powershell.exe -inputformat none %{FILE:samplepowershell.ps1} test example result
```
In this monitor, we use the "@powershell.exe -inputformat none" to specify that we are launching the following script through Powershell. In this scenario, we embedded a Powershell script in our template, viewable at the template root level. We also added arguments (test example result) which will be added to the output of the script ($args[0] $args[1] $args[2]). This functions exactly like it typically would for powershell scripts.

Sample output:
```
This is the output of my powershell script. My arguments specified
 in the command line are test, example and result.
```
<strong>Command Line Monitor - Powershell Command Host File</strong>

Command run on host:
```bat
@powershell.exe -inputformat none %{FILE:samplepowershell.ps1} test example result
```
In this monitor, we use the "@powershell.exe -inputformat none" to specify that we are launching the following script through Powershell. In this scenario, we are using a Powershell script located on the host system. We also added arguments (test example result) which will be added to the output of the script ($args[0] $args[1] $args[2]). This functions exactly like it typically would for powershell scripts.

Sample output:
```
This is the output of my powershell script. My arguments specified
 in the command line are test, example and result.
```

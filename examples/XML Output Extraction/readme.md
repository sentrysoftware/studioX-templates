<strong>XML Output Extraction</strong>
====================================================
This template shows how to monitor the output of a XML file, then capturing specific objects for monitoring. We first capture the output of the XML file, then we pass it through XML Pre-Processing, which will convert it to a csv format. From here, we can create multiple instances, and extract specific objects using Value Map monitors, Numeric Extractions, etc.

<strong>Command Line Monitor - Sample XML</strong>

Command run on host:
```bash
cat %{FILE:sample.xml}
```
This monitor is the method with which we retrieve the XML file. In our case, we simply embedded a XML file to the template (at the template level). In your setup, you will be using a different monitor to do so. This template was made to demonstrate what is done after we've collected the XML file, so we will not be going over all the different methods of obtaining said XML file.

Sample Output:
```XML
<?xml version="1.0" encoding="UTF-8" ?>
<root>
  <accounts>
    <userId>1</userId>
    <firstName>Krish</firstName>
    <lastName>Lee</lastName>
    <accountLocked>True</accountLocked>
    <passwordExpiresIn>32</passwordExpiresIn>
    <daysSinceLastLogin>1</daysSinceLastLogin>
  </accounts>
  <accounts>
    <userId>2</userId>
    <firstName>Racks</firstName>
    <lastName>Jacson</lastName>
    <accountLocked>False</accountLocked>
    <passwordExpiresIn>63</passwordExpiresIn>
    <daysSinceLastLogin>1</daysSinceLastLogin>
  </accounts>
</root>
```
<strong>Text Pre-Processing - XML Pre-Processing</strong>

This monitor will be used to convert the XML in a different format, in this case CSV. This will enable us to convert each line into Dynamic Instances further down the line. We set our XML Record Tag to accounts and our properties to userID;firstName;lastName;accountLocked;passwordExpiresIn;daysSinceLastLogin, to match the Record Tag of the XML file as well as specifying which properties we want included in our CSV. Finally, we set our result separator as ";", which will be the separator used in our CSV output.

<strong>Dynamic Instances - User Account Instances</strong>

In this monitor, we use dynamic instances to create one Monitoring Studio X instance per CSV line. This way, we will be able to separate all of the instances, so that each can be monitored independently. By specifying the separators earlier, we can now set our Column Separators as ";". Since several set of names could theoretically contain duplicates, we opted to use multiple columns to name each instance.

<strong>Value Map - Account Locked</strong>

This monitor is used to create various status based on the content of a specific column.  Similarly as the above monitor, we need to set the Column Separator to ";". We used column 5 which matches with "accountLocked". We set True as an alert, False as "OK" and anything else as "suspicious".

<strong>Numeric Extraction - Password Expires in (Days)</strong>

This monitor is where we will extract the PasswordExpiresIn value and set whichever alerts we may want. Similarly as the above monitor, we need to set the Column Separator to ";" and then specify the value as being in column number 6. In this example, we set the warning threshold at 7 days or above and the alarm threshold at 100%.

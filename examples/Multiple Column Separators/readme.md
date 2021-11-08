<strong>Multiple Column Separators</strong>
====================================================
This template shows how to set multiple column separators. This is a very basic scenario where for some reason, each line has a different separator, perhaps due to the merging of several files, or any other reason that may come to mind. In the Dynamic Instance monitor, we have configured all of these separators so that our data output could be separated properly.

<strong>Command Line Monitor - Sample File</strong>

Command run on host:
cat %{FILE:sampleoutput.txt}

This monitor is the method with which we retrieve our output to be parsed. In our case, we simply embedded a test file to the template (at the template level). In your setup, you will be using a different monitor to do so. This template was made to demonstrate what is done after we've collected the output, so we will not be going over all the different methods of obtaining said output.

Sample Output:
Name1:Test1
Name2>Test2
Name3=Test3

<strong>Dynamic Instances - Dynamic Examples</strong>

In this monitor, we use dynamic instances to create one MSX instance per line from out output. This way, we will be able to separate all of the instances, so that each can be monitored independently. We used 3 separate column separators (":","=" and ">" ). This can be useful when data is obtained and concatenated from several sources, or simply if we have several different separators in any given line. Any sub-monitors beyond this one will also require to have the same separators set to function properly.

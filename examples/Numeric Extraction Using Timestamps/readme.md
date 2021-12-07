<strong>Numeric Extraction Using Timestamps</strong>
====================================================
This template shows how to use the numeric extraction function to read a scientific notation format number and convert it to a decimal value in order to monitor and alert as applicable.

<strong>Command Line Monitor - Timestamp Output</strong>

Command run on host:
```bash
echo Value:9.99e+30
```
This monitor is the method with which we retrieve our output to be parsed. In our case, we simply used echo to receive an output to parse in the next monitor. In your setup, you will be using a different monitor to do so. This template was made to demonstrate what is done after we've collected the output, so we will not be going over all the different methods of obtaining said output.

Sample Output:
```
Timestamp: 01/01/2021 00:09:00
```
<strong>Numeric Extraction - Timestamp Extraction</strong>

This monitor is where we will extract the timestamp and calculate the time difference with the current time. To do so, we changed the Value Type to Timestamp and set the Value Parameter as "Time Elapsed From Now". Addtionally, we inputted our timestamp format "%d/%m/%Y %H:%M:%S". As this will output a result in seconds, we opted to convert it into days by dividing it by 86400 (24x60x60).

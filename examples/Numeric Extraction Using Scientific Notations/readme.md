<strong>Numeric Extraction Using Scientific Notations</strong>
====================================================
This template shows how to use the numeric extraction function to read a scientific notation format number and convert it to a decimal value in order to monitor and alert as applicable.

<strong>Command Line Monitor - Scientific Notation Output</strong>

Command run on host:
```bash
echo Value:9.99e+30
```
This monitor is the method with which we retrieve our output to be parsed. In our case, we simply used echo to receive an output to parse in the next monitor. In your setup, you will be using a different monitor to do so. This template was made to demonstrate what is done after we've collected the output, so we will not be going over all the different methods of obtaining said output.

Sample Output:
```
Value:9.99e+30
```
<strong>Numeric Extraction - Numeric Extraction</strong>

This monitor is where we will extract the scientific notation and set whichever alerts we may want. The important thing to note is that we enabled the option "Accept Scientific Notation". To be able to use alerting against this value, we divided it by 1e+28, leaving us with a value without scientific notations.

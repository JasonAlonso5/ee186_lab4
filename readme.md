What are the different bit resolutions can you set the ADC? What is the maximum sampling rate at each of these resolutions? Where did you find this information in the datasheet? 
You can set the ADC to 12, 10, 8, or 6-bit resolution. The max sampling rates for fast channels are 5.33, 6.15, 7.27, and 8.88 Msps, respectively. 
For slow channels, the max sampling rates are are 4.21, 4.71, 5.33, 6.15 Msps, respectively. I found this information in table 81, ADC characteristics, in section 6.3.21.

Why do you need a voltage divider circuit? What would happen if the photodiode is directly connected to the board? 
A voltage divider circuit is necessary because the photodiode produces a current. By Ohms law, we need a resistor in order to convert the current into measurable voltage. 
If we connected the photodiode directly to the board, then the ADC pin's input impedance will prevent any current from flowing through. 
Thus, the voltage value we read would not be accurate and it would not change based off of the photodiode's output.

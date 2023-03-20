# Transparent_bridge_1.0

Its a **Transparent_brigde**, which is use to send the bytes comming from network layer using mqtt protocol to Serial communication (RS-485) and From  Serial communication (RS-485) bytes to Mqtt topics

## Features

some basic features for this module are . 
- It can retain counter value if controller softreset for any reasons.


## PARAMETER
There are some parameter for setting the module which are discuss below
- **Slave_ID**: It is use to give device an ID which is in range (1-255) . Default is **1**
- **Serial_Configuration**:  Device have some selected Serial configuration Defaults 
is **wordlenght** = 8 **parity** =none  **stop bits** = 1
- **Serial_Baud**:  device have some selection of baudrate which are 2400,4800,9600,19200,38400 Default is **9600**
- **Network_timeout**:  Network timeout use to set the status led for how long it turn off when command recieves (its in milliseconds)
- **Debounce_time**:  Debounce time is use to set the debounce for the input button Default is **200**
- **Count_1**:  Count_1 are use to set the offset to the counter so that the count of input_1 will start increament from the offset which set  Default is **0**
- **Count_2**:  Count_2 are use to set the offset to the counter so that the count of input_2 will start increament from the offset which set  Default is **0**
- **EPOCH**:  Epouch is use for setting the current time in second to the controller so that controller sync to current time and Default is **0** from the power on 

## Communication Use

2 commication interface are using 
- Rs-485 module for physical interface
- Ethernet module for Network interface

## OUTPUT RELAY

2 output relays are connected to the module
- Output Relay_1 is connected to pin PB0
- Output Relay_2 is connected to pin PB0

## STATUS LED

Status led is connected to pin PC13

## Communication Protocol

This module has 2 commincation Protocol 
- USB protocol for Serial Debugging
- RS-485 Serial Interface for Modbus commands

## Operating Voltage

The operating voltage for this module is 5 volts

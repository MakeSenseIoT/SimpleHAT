## MakeSenseIoT SimpleHAT

<img src="assets/SimpleHAT.jpg?raw=true" width="500px"><br/>


PCB files for the SimpleHAT by MakeSenseIoT  

Format is EagleCAD schematic and board layout


### Hardware

The SimpleHAT is a Raspberry Pi Zero W HAT with multiple functionalities. 
It can operate as a standalone unit or as a part of more complex system, for example
Solar Powered IoT camera. 
The SimpleHAT hardware includes:

* Circutry for powering ON/OFF Raspberry Pi using external signal 
* Placeholder for Raspberry Pi Camera module
* Placeholder for 0.91" OLED display module
* Placeholder for 1.3" OLED display module
* Placeholder for UART to USB converter
* Placeholder for I2C (QWIIC)

Note: Due to physical limitation, not all hardware options can be used togrther

### RPI Software
* ON/OFF

For ON/OFF functionality use Pimoroni one-line installer for daemon configuration:

```
curl https://get.pimoroni.com/onoffshim | bash
```
 **IMPORTANT** Do not use pushbutton while using external signal for ON/OF
as it might result in damaging of external driving circuitry. There is no protecting
circuit to prevent it. Use only one ON/OFF source at a time.

* I2C OLEDs
There are multiple online tutorials and example code available online 

* Raspberry Pi Camera UV4L 
There are multiple online tutorials and example code available online. We use UV4L - for installation details
see [UV4L](https://www.linux-projects.org/uv4l/installation/)


## Authors

* **Jan Szymanski** - *Initial work* - [MakeSenseIoT](http://www.makesenseiot.com)

## Acknowledgments

* The OnOff SHIM code by Pimoroni is used
* Inspired by Pimoroni project updated and modified [Pimoroni](https://shop.pimoroni.com/products/onoff-shim)


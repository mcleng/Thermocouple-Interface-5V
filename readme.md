Thermocouple Interface | 5V
===========================

This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/">Creative Commons Attribution-ShareAlike 3.0 Unported License</a>.

<a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-sa/3.0/88x31.png" /></a>
	
Designed By:

*	Ryan McLaughlin <ryan@ryanjmclaughlin.com>


Summary
-------

The single thermocouple interface was made out of the need to interface a micro controller to a thermocouple. One of the popular chips to perform a thermocouple to digital conversion is the MAX6675 (now MAX31855). While this is a great little chip it is a small surface mount part and therefore difficult to solder. The thermocouple interface board not only helps with having the chip broken out to a simple 0.1" header, but also provides a mini-thermocouple connector to easily interface to a thermocouple. Thermocouples are not designed to be soldered and this provides a good solid connection, while also using the proper metals in the connector required for a thermocouple connection.

This version of the board is a 5V compatible version of the interface. It is equipped with a MAX31855, along with the necessary voltage regulation and level shifting to allow for it to be directly hooked up to a 5V micro controller similar to an Arduino. The board comes fully assembled and includes a male and female header. Licensed under OSHW


Tutorial
--------

It is simple to get everything up and running.

1.	Install a header or solder jumper wires to the pin connections
2.	Connect a K-Type [Thermocouple](http://en.wikipedia.org/wiki/Thermocouple Thermocouple) to the PCB Thermocouple Connector use a Thermocouple Wire Connector if necessary
3.	Wire the necessary connections to an Arduino or other micro controller, the bare minimum connections are +V, GND, SCK, SO, CS
4.	If using an Arduino, load one of the samples from the MAX6675 Arduino Library and you should see temperature information in the serial console. With other micro controllers you can access the chip using a standard SPI interface. See MAX31855 data sheet for more details.


Board Specs
-----------

*	Dimensions: 1.25" x 1.50"
*	Chip: MAX31855, TXB0104
*	Voltage: 5V
*	Header: 1x6 0.1" Pitch
*	Fixturing: Four Corner Holes (1.20"x0.95" Spacing)


Versions
--------

###v2.0

Initial release of a 5V board with on-board level shifter. Other changes included:

* Initial release under Eagle 6.1 on Github
* PCB Production dates: 09-2011


Purchase
--------

[store.ryanjmclaughlin.com](http://store.ryanjmclaughlin.com). 


TODO
----

*	Do not route LED through level shifter

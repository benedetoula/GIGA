# Welcome to GIGA Node

The GIGA Node is a design object meant to communicate through light and form the level of connectivity experienced by Schools around the Globe with the objective of promoting transparency, accountability, and access in all Schools connected through GIGA. GIGA is a partnership between UNICEF and ITU that aims to connect every school to the Internet, and every young person and their community to information, opportunity and choice. 

## Hardware

When designing the GIGA Node we were really focused on making sure every part of the system was replaceable and serviceable while also minimizing the number of components used as much as possible, to simplify sourcing and maintenance.

![Image](System%20Diagram2.png)

The Hardware design is mainly comprised of 3 elements:
- **The Light Indicator:** this is a custom LED matrix that showcases the level of connectivity available.
- **The Node:** this is the brain of the system, which runs speedtests, geo-location, a blockchain node and WiFi hotspot.
- **The Power Electronics:** this includes a 15W photovoltaic panel (PV), a charge controller to properly charge the battery and all DC/DC converters needed to regulate the power to the Node.

![Image](System%20Diagram.jpeg)

The enclosure of the GIGA Node was entirely custom designed and built to be adjustable, portable and transportable in a standard size carry-on for easy travel!

For a detailed [*Bill Of Materials*](https://docs.google.com/spreadsheets/d/1M344BFzDwndOonXr7UBz_JfK02XLmgQRAvrM4X4WKnk/edit#gid=0) please check this document.

## Firmware 

The GIGA Node firmware is built on Linux OS and includes custom code to: 
- routinely check for Quality of Service of Internet connectivity 
- geolocate the unit through its assigned IP address
- generate a public WiFi hotspot (currently limited to 7 devices)
- control the LED Light Indicator module and create light animations to visually communicate each stage of the Node activities
- and run a blockchain node to permanenty store and archive data from the speedtests.   


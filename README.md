IPPNAR - Intelligent Path Planning and Navigation for Autonomous Robots
=================

This is the readme file for IPPNAR. 

This project was undertaken by me and my friends as part of our undergraduate
course in Information Science and Engineering. The goal of the project was to
construct an autonomous rover which could navigate through a set of waypoints
provided as GPS coordinates while avoiding any obstacle encountered. The goal
was also to keep the rover on the road.

More information can be found as comments in source or at http://by2.in/ippnar

Contents
--------
 - License
 - Hardware requirements
 - What is in this package
 - Dependencies
 - Building from source
 - Getting help

License
-------

This project is distributed under the terms of the Apache Software Foundation
license, version 2.0. The text is included in the file LICENSE in the root
of the project.

Hardware requirements
------------------------------------

This project was developed on Eclipse CDT running on a Fedora 8 machine.

Parts used:
 - Fedora 8 running on Dell Studio
 - AVR Mega8 x 3
 - Compass module from Sparkfun Electronics
 - Nokia smartphone with GPS, Bluetooth and J2ME support
 
Please note that the parts mentioned above are in no way exaustive, and
definitely not rigid. Almost all parts can be removed easily with minimal
changes to code.

What is in this package
-----------------------

This package contains the source code of core control module and other helper
modules.

You will find the source code here:

	|-- CommandModule
	|-- CompassReader
	|-- GPS_J2ME_Applet
	`-- MotorDriverUnit

Here is a list of projects in this distribution and what they do.

 - CommandModule: the core project, includes the blackboard and control module;
 - CompassReader: contains microcontroller code to read the compass;
 - GPS_J2ME_Applet: contains a J2ME application to read GPS data and transmit over
   bluetooth to command module;
 - MotorDriverUnit: drives the robot based on instructions from command module;

Dependencies
------------

The dependencies have been include in source.

Here is a break down of the dependencies we use. For the complete and precise
reference read below.

 - AVR GCC:

    compiler for AVR C (http://www.nongnu.org/avr-libc/)

 - OpenCV:

 	from Willow Garage (opencv.willowgarage.com)

 - BlueZ:

    for bluetooth communication (http://www.bluez.org/)

 - LibUSB:

    for linux (http://www.libusb.org/)

 - POSIX Threads:

    with GCC (http://gcc.gnu.org/)

 - V-USB:

    from Obdev (http://www.obdev.at/products/vusb/index.html)

Building from source
---------------------------

to be updated later

Migrating from 1.4
------------------

This file is a copy of the migration guide from available on our Wiki:

    http://cwiki.apache.org/WICKET/migrate-15.html
    
Getting help
------------

 - Ask around on StackExchange Robotics site

 - Read the manuals

 - Ask at Obdev forums

 - Send a complete message containing your problem, stacktrace and problem
   you're trying to solve to me (abhi [at] by2 . in)
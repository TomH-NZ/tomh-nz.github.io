---
layout: post
title: Enum Basics in C#
---

### Enum Basics in C#!

Enum (Enumeration) is a value type, similar to _int_, _string_ and _decimal_.  The _enum_ is defined by using the _enum_ keyword and then specifying the enum members.  For example:

![Example code showing the setup of an Emum]( https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Enum_Example_001.jpg "Example code showing the setup of an Emum")


Each entry in the enum is mapped to an integer that represents its location in the enum list.  For example:

![Example code showing an Enum being called by its integer]( https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Enum_Example_002.jpg "Example code showing an Enum being called by its integer")


Running this code will result in "East" being displayed. (0 - North, 1 - East, 2 - West, 3 - South).

It is possible for the enum member to have a different integer location then default.  For example:

![Example code showing an Enum with a different location integer]( https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Enum_Example_003.jpg "Example code showing an Enum with a different location integer")


To print the integer values to console you would use the following code:

![Example code showing Console Writeline instructions]( https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Enum_Example_004.jpg "Example code showing showing Console Writeline instructions")

The results of the above code will be:

 _North, 0_.
 
 _East, 20_.
 
 _West, 30_.
 
 _South, 31_.



_North_ has an integer value of 0 because it is first in the list and has not had its value changed, unlike _East_ which has had its integer value assigned as 20.  _South_ has an integer value of 31 because it follows on from _West_, which has been assigned an integer value of 30.

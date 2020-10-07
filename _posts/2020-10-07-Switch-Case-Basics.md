---
layout: post
title: Switch Case Basics in C#
---

### Looking at Switch/Case basics in C#

In C# Switch statements are used to execute blocks of code, depending on which Case value the statement matches.  They can be used in place of If/Else to make your code cleaner and easier to read.  For example:

![Switch/Case example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Switch_Case_Example_001.jpg "Switch/Case example")


In the above example the code will set the parameter _value_ to _5_, and then run it through the Switch statement.  When the correct Case matches the value, it will run that code, printing out "The number is 5" in this example.

When using a switch statement most value types, such as _int_ and _char_, can be used.  If a string is used in the switch statement the system will convert it to a hidden dictionary when processing the case pattern.

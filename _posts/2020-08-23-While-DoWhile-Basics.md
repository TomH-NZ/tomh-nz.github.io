---
layout: post
title: While / Do-While Basics in C#
---

### Looking at While / Do-While loop basics in C#

A While loop runs through a block of code until a specified condition is met. When the condition is met, the loop exits. For example:

![A While example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/while_example_001.jpg "Basic While example")

The above code will execute while the variable _index_ is less than 5. When _index_ reaches 5, the loop will exit out.  It is possible for the loop to not run at all, if the condition is met before the code enters the While loop.  For example:

![An invalid While example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/while_example_002.jpg "Invalid While example")

This _while_ loop will not run as the condition (_index < 5_) is met at the start of the code block.


A Do-While loop will always run at least once, as it executes the code block before checking of the condition has been met or not. For example:

![A Do While example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/do_while_example_001.jpg "Basic do while example")

This do/while loop will run once as it checks if _index < 5_ at the end of the code block, after running the _Console.WriteLine_ command.


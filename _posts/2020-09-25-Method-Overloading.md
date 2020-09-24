---
layout: post
title: Method Overloading in C#
---

### Method Overloading Basics in C#!

Method overloading in C# is an action where two methods can have the same name, yet different input parameters. For example:

![Overloaded method creation example]( https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Method_Overload_Example_001.jpg "Overloaded method creation example")


Although the two methods have the same name and number of input parameters, because the input types are different the code will be treated as two different methods when it is run, depending on the input entered at runtime.

![Example code showing overloaded methods in use]( https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Method_Overload_Example_002.jpg "Example code showing overloaded methods in use")


Running the above code will generate two different results, depending on what the input parameter type is for the method.

An example of overloading that will not work is:

![Invalid overloaded method example]( https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Method_Overload_Example_003.jpg "Invalid overloaded method example")

Although the output types of the methods are different, because they have the same name and same number of input parameters the code will generate an error when it is run.

Method overloading can be used in situations where a user input needs to handle different paramters types.

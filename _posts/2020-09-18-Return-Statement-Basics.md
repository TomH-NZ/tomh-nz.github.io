---
layout: post
title: Return Statement Basics in C#!
---

### Looking at Return Statement basics in C#.

A Return statement is used in C# to terminate the execution of a method/function that it is in and return control to the method that called it.

_Return_ can also be used to return an optional value, based on the type of method that it is used in.  For example:

![A method with a return statement example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Return_Statement_Example_001.jpg "Basic method with a return statement example")


The above method will take in two integers (_x_ and _y_), add them together and then use the _return_ statement to return the resulting variable _number_ to the method that called it.

If the return type of the class or method is _void_ then it is possible to run the class/method without having a _return_ statement.  For example:

![A method without a return statement example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Return_Statement_Example_002.jpg "Basic method without a return statement example")


The above code will run and print out "No return necessary" in the console.  As the return type is _void_, there is no need for a return statement for this to work.

---
layout: post
title: Object Constructor Basics in C#
---

### Looking at Object Constructor basics in C#

In C# a constructor is a method that is used when an object is instantiated, passing values and fields for the object to use.  For example:

![A Constructor example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Constructor_example_00111.jpg "Basic Constructor example")

This code creates a new object called Car.  The constructor (highlighted in the red box) passes the parameters (model, numberOfWheels) to the object when it is instantiated, so that the user can use the parameters in the code (Chevrolet.model = "Corvette", Chevrolet.numberOfWheels = 4).

One important thing to note is that the name of the constructor **must** match the name of the class, and it cannot have a return type, such as void, int, etc.

With the constructor it is possible to pass default values for the parameters, which can be overloaded when the object is instantiated.  For example:

![A Constructor with defaults example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Constructor_example_0012.jpg "Basic Constructor with defaults example")

When a new Car is created, if there is no value specified for numberOfWheels then the default value of 2 will be used.  One thing to note when setting up default values in the constructor is that any parameters which are assigned values are placed after parameters without value, i.e: the parameter _numerOfWheels_ is placed after _modeName_ as it has a default value of 2 specified.


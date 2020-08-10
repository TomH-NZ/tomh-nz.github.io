---
layout: post
title: Static Class Basics in C#
---


### Static Class Basics in C#

In C# the _static_ modifier is used to determine how a class can be accessed.

If _static_ is used in a class, then the class cannot be instantiated and the class name is used to access anything inside the class.

![A static class example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/FizzBizz_Class_example_001.jpg "Static class example")

Because the class FizzBuzz has _static_ as a modifier, to access the Calculator method inside it you would only need to call FizzBuzz.Calculator.  An example of this would be:

![Calling a static class example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/FizzBizz_Class_example_002.jpg "Calling a static class")

If the class did not have _static_ as a modifier then you would need to use the _new_ key word to create the object, so that the methods inside it can be used/accessed.
For example:

![Non-static class example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Car_Class_example_001.jpg "Non-static class example")

As the class Car does not have _static_ as a modifier, to access any of the methods inside it (model, color, year) you need to instantiate the class first by creating a new object, in this case Ford, and then calling the methods afterwards.  When the class is instantiated the values for _model_, _color_ and _year_ are provided to it.

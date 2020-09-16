---
layout: post
title: XUnit Unit Test Constructor Basics
---

### Looking at constructors in XUnit Unit Testing in C#.

In unit testing with XUnit, if there is an object that you are using regularly in tests in a class, then it is possible to create a constructor for that object so that you do not need to create it in every test that uses it. For example:

![A constructor example in XUnit](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Xunit_Test_Constructor_Example_001.jpg "A constructor example in XUnit")


In this example, the class used in testing is _GameConfigShould_ with the object that is being used called _player_ of the type _Player_.  The constructor follows the same rules as a constructor used in the normal code in that it has the same name as the class that it is created in, with no return type, and creates the new object to be used in the unit tests.

With the player object having been created it can now be used in the tests by using calling it as normal, giving access to any of the methods that are part of the player object.  This is shown in the example by the _Assert.Equal_ line calling _player.Health_ as the actual result of the test.

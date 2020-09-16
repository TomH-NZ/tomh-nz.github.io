---
layout: post
title: Constructors in XUnit Unit Tests!
---

### Looking at constructors in Xunit unit testing.

In unit testing with Xunit, if there is an object that you are using regularly in tests in a class, then it is possible to create a constructor for that object so that you do not need to create it in every test that uses it.  For example:

![A constructor example in XUnit](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Xunit_Test_Constructor_Example_001.jpg "Basic constructor example in XUnit")


In this example the class used in testing is _GameConfigShould_ with the object that is being used called _player_ of the type _Player_.  The constructor follows the same rules as a constructor used in the normal code in that it has the same name as the class that it it created in, with no return type, and creates the new object to be used in the unit tests.

With the _player_ object having been created it can now be used in the tests by calling it as normal, giving access to any of the methods that are part of the _player_ object. This is shown in the example by the _Assert.Equal_ line calling _player.Health_ as the actual result of the test.

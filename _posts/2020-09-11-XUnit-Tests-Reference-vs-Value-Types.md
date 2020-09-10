---
layout: post
title: Xunit Tests - Reference vs Value Types
---

### How Reference types differ from Value types in XUnit Tests in C#.

In C# the two main data types that are used are Reference types and Value types, with the difference between them being in how they store the values in the computer memory. It is this difference that has the potential to cause issues with testing in XUnit.


![An integer unit test example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/XunitTest_Int_Example_01.jpg "An integer unit test example")


The above test compares an _integer_ value to an _integer_ value, which will work correctly.  As an _int_ is a Value type the testing software compares the info that is stored in the _int_ memory location, which is the actual value of the integer itself.


![A class unit test example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/XunitTest_Class_Example_01.jpg "A class unit test example")


The test above will fail as the two objects being tested (classes created from the Player class) are Reference types.  When Xunit tests compares the two reference types it does not see the values that the two classes represent and instead compares the reference values stored in the memory location that the class is mapped to.  As the two reference values are different the unit test will fail.

The only exception to this is unit testing with _strings_.  Although a _string_ is a reference type, when they are used in XUnit testing they are considered as value types and can therefore be used for direct comparisons.  For example, the following test will successfully pass unit test:



![A string unit test example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/XunitTest_String_Example_01.jpg "A string unit test example")

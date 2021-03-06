---
layout: post
title: Array Basics in C#
---

### Looking at single dimensional Arrays

Arrays are data structures in C# that can hold multiple variables of the same type of data, with the datatype being specified when the array is instantiated. The three types of arrays are single dimensional, multi-dimensional and jagged arrays.
This post will look at single dimensional arrays, with future posts looking at multi-dimensional and jagged arrays.


Single dimensional arrays are used to store data that can accessed by functions and methods in C#, with the datatype of the array being set when the array is created and the numbering sequence of the elements starting from zero.


When the array is created you specify the datatype and number of elements in the array, if you are not adding the data at that time. Eg:

![New string array example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/new_string_array_example_001.jpg "New string array example")

The example above creates a string array with a length of 5, with the elements numbering from exampleStringArray[0] through to exampleStringArray[4]. The contents of the array can be added at the time the array is instantiated in multiple ways.

Example 1:

![New string array example with data](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/new_string_array_example_002.jpg "New string array example with data")

This creates a new array with 7 elements, each element being a string.

Example 2:

![New integer array example with data](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/new_integer_array_example_001.jpg "New integer array example with data")

This example creates an array with 6 integer elements at the time that the array is instantiated. Even though the number of elements is not specified in the array C# is able to infer the number of elements from the data that is being fed into it.


To call the element in the array you would need to specify the array name, as well as the location of the element, with the numbering of the elements starting from 0. For example:

![Console write of string array data example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/string_array_console_example_002.jpg " Console write of string array data example")

This would call the 2nd element in the array, Tues, as the numbering goes [0] = "Mon", [1] = "Tues"  .... [6] = "Sun".

---
layout: post
title: C# Array Basics
---

## Array Basics in C#.

Arrays are data structures in C# that can hold multiple variables of the same type of data, with the datatype being specified when the array is instantiated. The three types of arrays are single dimensional, multi-dimensional and jagged arrays.
This post will look at single dimensional arrays, with future posts looking at multi-dimensional and jagged arrays.


Single dimensional arrays are used to store data that can accessed by functions and methods in C#, with the datatype of the array being set when the array is created and the numbering sequence of the elements starting from zero.
When the array is created you specify the datatype and number of elements in the array, eg:

```
string[] exampleStringArray = new string[5];
```

The example above creates a string array with a length of 5, with the elements numbering from exampleStringArray[0] through to exampleStringArray[4].  

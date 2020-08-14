---
layout: post
title: Jagged Array Basics in C#
---

### Jagged Array Basics

Previous posts have looked at single dimension and multidimension arrays in C#, and this post will look at the basics of creating jagged arrays.

The easiest way to think of a jagged array is that it is an array of arrays, in that each element of the parent array is an array itself.  Creation of the jagged array follows the same principles the other types, with the length of the sub-array not being required if you are specifying the data at the time of instantiation.

For example: 

![New jagged array example]( https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/new_jagged_array_example_001.jpg "New jagged array example" )

This command creates a jagged array containing 3 elements (arrays).  To initialise the elements of the jagged array you would need to specify each element individually.

![New jagged array elements example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/new_jagged_array_example_002.jpg "New jagged array elements example" )


As with the single and multidimension arrays, it's possible to initialise the sub-arrays without specifying the array length, as long as the data is included.

![New sub-array example with data](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/new_jagged_array_example_003.jpg "New sub-array example with data")


With the instantiation rules of arrays it's possible to combine the creation of all the elements of a jagged array in one step:

![New jagged array creation with sub-array elements](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/new_jagged_array_example_004.jpg "New jagged array creation with sub-array elements")

This example creates a jagged array of the string type, with 4 string arrays inside, with each array having lengths of 5, 4, 3 and 3 respectively.

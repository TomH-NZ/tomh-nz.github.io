---
layout: post
title: Multidimension Arrays in C#
---

### Multidimensional Array Basics!

In the [previous post](https://tomh-nz.github.io/Array-Basics/) I went over how single dimension arrays are created, what they can be used for and how they are read by the code.  Another variation of arrays is the multidimensional array, which differs from single dimension arrays in that it can store multiple bits of data per element, rather than a single bit.

When a multidimensional array is created it has at least two values specified. The first value is the number of columns in the array, the second value the number of rows in each column, the third being the number of segments in the row, etc.
The following example creates an array with 4 columns and 2 rows per column:

![2D multidimensional array example with data]( https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/new_multidimension_integer_array_example_001.jpg "2D multidimensional array example with data")


To create an array with more than 2 dimensions you would specify the details at the time of creation.  For example, an array with 2 columns, 2 rows and 3 segments would look like:


![3D multidimensional array example with data]( https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/new_multidimension_integer_array_example_002.jpg "3D multidimensional array example with data")



When calling the data contained in the array you would need to pass the location information for the element, otherwise an error will be returned.  For example, to call the first element of a 2 dimensional array:

![2D multidimensional array console write example]( https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/multidimensional_int_array_console_example_002.jpg "2D multidimensional array console write example")

This returns the value of **1** (column 0, row 0).

To call the data in an array with more than 2 dimensions you would use:

![3D multidimensional array console write example]( https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/multidimensional_int_array_console_example_001.jpg "3D multidimensional array console write example" )

This call returns the value of **12** (column 1, row 1, segment 2).


An example of the use of multidimensional arrays would be positions on a game board, chess for example.  You could store the starting positions for various tokens using the columns and rows as the coordinates.

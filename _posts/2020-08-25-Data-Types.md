---
layout: post
title: Data Types Basics in C#
---

### Looking at Data Type basics in C#

In C# there are two main data types that are used, value types and reference types, with the difference being in the way that each type stores it's data in the system memory.

Value types store the assigned value in the memory space assiged to the variable. For example:

_int i = 10;_


Integer _i_ has been assigned the memory address 0x80123.  If you were to look into that space in the memory the value of '10' would be stored inside.  When a program uses the int _i_ it reads the memory address directly, acting on the data in the memory address from there.

Examples of Values Types in C# are:
* bool
* decimal
* double
* char
* int
* enum
* float
* struct

Instead of storing the actual data, Reference types instead store the memory location of the data, effectively pointing towards the data.  For example:

_string s = "Hello World!";_


The string _s_ has been assigned the memory address 0x80987, however if you look into that address in the memory you would see another memory address, 0x30987.  The new address, 0x30987, is the actual storage location for the "Hello World!" data.

Examples of Reference ypes in C# are:
* string
* class
* array _*_

_*_ Note: Arrays are considered reference types, even though the data they contain may be a value type.

---
layout: post
title: If/Else Basics in C#!
---

### Looking at If/Else statement basics in C#.

If/else statements in C# are used to execute blocks of code based on if an expression evaluates to true.
For example:

![An if/else example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/IfElse_Example_001.jpg "Basic if/else example")

When the above _If_ statement is run it looks at the first condition ( is _value == 1_ true?) , decides that _value_ is not equivalent to 1 and runs the _else_ statement.

If you have multiple expressions for the statement to test against, you would use the _else if_ statement after the initial _if_ statement.
For example:

![An if/else if/else example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/IfElse_Example_002.jpg "Basic if/else if/else example")

This example  will check the condition in each statement against the original value and run the code when they match.

It is also possible to have a nested _if/else_ statement within an existing _if/else_ statement.
For example:

![A nested if/else if/else example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/IfElse_Example_003.jpg "A nested if/else if/else example")

The above code will first check each statement to see if it is the equivalent of 3, when it finds a match it will then run the second _if/else_, checking if the variable color is the equivalent of _blue_.

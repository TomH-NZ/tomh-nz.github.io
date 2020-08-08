---
layout: post
title: Ternary Operator Basics in C#
---

### Ternary Operator Basics

 The conditional operator "_? :_" , or Ternary operator, is used in C# to replace short if/else statements and make the code cleaner and more human readable.  It does this by looking at a Boolean expression and returning one of two results, depending on whether the expression evaluates to true or false.

 A basic way of looking at it like this:
 _is this condition true ? yes - return first value : no - return second value_
 
 An example of a ternary operator is:
" _5 > 3 ? Five is greater than three : Five is less than three_ "
This line would return the value of "_Five is greater than three_", as the condition _5 > 3_ would evaluate to true, so the system returns the first value.

" _5 > 10 ? Five is greater than ten : Five is less than ten_ "
In this example _5 > 10_ would evaluate to false, so it would return " _Five is less than ten_ ".


It is possible to nest a ternary operator inside another ternary operator.  For example:
_int x = 5, y = 10, z = 7_

_int result x > y ? x : y > z ? y : z_

When the code is run through it is looked at by the system as _x > y ? x : (y > z ? y : z)_.
The operator would first check if x is greater than y, returning the second part of the operator since 5 is not greater than 10. At this point it would run the nested ternary operator,  _y > z ? y : z_, checking if 10 is greater than 7.  As 10 is greater than 7 the first result of the second operator, _y_, would be returned by the code.

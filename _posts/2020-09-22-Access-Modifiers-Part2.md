---
layout: post
title: Access Modifiers in C# - Pt 2
---

### Access Modifiers in C# Pt 2

As mentioned in a [previous post](https://tomh-nz.github.io/Access-Modifiers-Part1/) there are 4 commonly used access modifiers in C#: Public, Private, Internal and Protected.  In my previous post I looked at Public and Private, in this one I shall be looking at Internal and Protected.

If a method has the _internal_ access modifier it can only be accessed by objects within the same namespace or assembly (executable or dynamic link library) as the method.  For example:

![An Internal access modifier example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Access_modifier_Internal_001.jpg "Internal access modifier example")


As _BaseClass_ is public, it can be accessed from anywhere, both from classes/methods inside MyProgram.exe as well as from AnotherProgram.exe.  However when AnotherProgram.exe tries to access the internal object _intObject_ it will get an access violation error message.

The _protected_ access modifier is similar in that it can only be accessed by objects within the same class as the protected object, or by classes which are derived from the base class via inheritance.  For example:

![A protected access modifier example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Access_modifier_Protected_001.jpg "Protected access modifier example")

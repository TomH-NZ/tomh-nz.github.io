---
layout: post
title: Access Modifiers in C# - Pt 1
---

### Looking at access modifiers in C# Pt 1

In C# access to the code is controlled by access modifiers which are added to the object when it is created.  The most commonly used access modifiers are _public_, _private_, _protected_ and _internal_.  This entry will be looking at the public and private modifiers, with internal and protected coming in another entry.


The _public_ access modifier is the most permissive of the modifiers used in C#, as it places no restrictions on how the public member is accessed.  This means that anything marked as _public_ can be accessed from a different method, a different class or a different program entirely.  For example:


![A public access modifier example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Access_modifier_Public_001.jpg "Public access modifier example")

As the objects _X_ and _Y_ are marked as public in TestClass they can be read and changed from anywhere, such as the separate class MainClass.  In MainClass the _X_ and _Y_ objects are assigned values and then used in the Console.WriteLine process.


The _private_ access modifier is more retricted than the _public_ modifier.  This means that any methods/functions marked as private can only be accessed from within the class that they were created in.  For example:


![A private access modifier example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Access_modifier_Private_001.jpg "Private access modifier example").

In the example the _name_ and _salary_ methods are marked as _private_, hence they can only be accessed by other methods from within the same class, the GetName() and GetSalary() methods.  The values represented by _name_ and _salary_ are available in MainClass because they are called  and set through GetName and GetSalary. If MainClass tried to access _name_ or _salary_ directly it would get an access violation error.

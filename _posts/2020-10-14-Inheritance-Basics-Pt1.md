---
layout: post
title: Inheritance basics in C#, Pt 1
---

### Looking at Inheritance basics in C#, Pt 1

In C# inheritance allows the user to create a new class that can use, extend or modify the functionality defined in another class.  The class which is inheriting the functionality is called the _derived class_, with the class being inherited from being called the _base class_.  For example:

![Example code showing the setup of a base class and a derived class]( https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Inheritance_Example_002.jpg "Example code showing the setup of a base class and a derived class")


The above example has _EvilRobot_ as the base class, which contains the methods _Fly()_ and _TerrorizeTheCity_, which are inherited by _RegularRobot_, the derived class.  The object created from the derived class (_robbie_) has access to the _Fly()_ and _TerrorizeTheCity_ methods that are contained in the base class.

![Example code showing a derived class accessing a method]( https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Inheritance_Example_001.jpg "Example code showing a derived class accessing a method")


With an inherited method it is possible to override it so that it has the same name as the original method, however the contents are different.  To do this you need to mark the _base_ method as virtual and the deriving method as _override_.  For example:

![Example code showing a derived class overriding a method]( https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Inheritance_Example_003.jpg "Example code showing a derived class overriding a method")


Creating the object _robbie_ and then calling the method _Fly()_ will print out "I am grounded." rather than "I am flying!", due to the _Fly()_ method being overridden in the _RegularRobot_ derived class.
If the overridden method is called by an object that is created from another class that inherits from the base class, the method will run the code as normal.

Although the base _Fly()_ method has been overridden in the derived class, it is possible to run the method in the derived class by the _base_ keyword from within the method in the derived class.  for example:

![Example code showing a derived class accessing a base method]( https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Inheritance_Example_004.jpg "Example code showing a derived class accessing a base method")

![Example code showing a derived object accessing a base method]( https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Inheritance_Example_005.jpg "Example code showing a derived object accessing a base method")

The output for the above code will be "I am grounded." for _Fly()_ and "I am flying!" for _Fly2()_.

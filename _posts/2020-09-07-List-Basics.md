---
layout: post
title: List Basics in C#!
---

### Looking at List basics in C#.

Lists in C# belong to the same family as Dictionaries, Arrays and HashSets.  _Lists_ are used to store objects in a list form that can be manipulated after it has been created, unlike an array which is set in stone when it is created.  This is useful for instances where data may be added or removed in the future, such as employees in payroll software, a student list in a classroom, etc.

When creating a list the format is similar to creating an array in that you give the list the objects at the time of instantiation.  For example:

![A new List example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/new_list_example_001.jpg "Basic new List example")


To display the items in the list you would use _list[i]_, with _i_ being the index of the item you wish to show, starting at zero for the first item in the list.

![Displaying an item from a list example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/new_list_example_002.jpg "Displaying an item from a List example")


The above code would display orange, as it is the entry that would correspond with the 2nd index.

To add additonal entries to the list you would use the _Add_ command.  For example:

![Adding items to a list example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/new_list_example_003.jpg "Adding items to a List example")


It is possible to add entries to the list at specific positions.  For example:

![Adding entries at a specific index example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/new_list_example_004.jpg "Adding entries at a specific index example")


The above example will create the list, add the color _red_ at the 2nd position (index 1) and then print out each color in the List.

Removing entries from the list uses a similar syntax:

_exampleList.Remove("orange")_ would remove the entry "orange" from the list.
_exampleList.Remove(0)_ would remove the first entry from the list (index 0).

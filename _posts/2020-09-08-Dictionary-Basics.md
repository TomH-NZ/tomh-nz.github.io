---
layout: post
title: Dictionary Basics in C#!
---

### Looking at Dictionary basics in C#.

In C# a Dictionary is similar to a List in that both store values, however in a Dictionary you can specify the key that is matched to the value, whereas with a List you can only specify the values.  Also, with a Dictionary the order of the entries is non-deterministic (meaning that the order isn't determined by anything), rather than being determined by the index.  For example:

![A dictionary example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Dictionary_Example_001.jpg "Basic dictionary example")


The above example will create a dictionary that has 4 entries in it.  The key for the first entry is "_Ford_", with the value for the entry being 100.  As every key in the dictionary has to be unique, if you tried to add another key-value pair with the key of "_Ford_" it would generate an error saying that the key already exists.
It is possible to have another key-value pair that has the value of 100 if the key being used is unique.  For example:

![A duplicate value example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Dictionary_Example_002.jpg "A duplicate value example")


Because the keys for the two entries that have the value of 100 (_Ducati_ and _KTM_) are unique, the system accepts them.

To retrieve the values from a dictionary, the most efficient way is to use the _TryGetValue_ method.  For example:

![A TryGetValue example](https://raw.githubusercontent.com/TomH-NZ/tomh-nz.github.io/master/images/Dictionary_Example_003.jpg "A TryGetValue value example")


The above code will return the result of 120, which is the value that matches to the key of "_BMW_".  Because _TryGetValue_ returns a bool (true/false) result, if you want to get the value then you need to specify an output object (_outputValue_ in this case) and then call that object from there.

To add or remove a key-value pair from a dictionary the process is similar.

_dictionaryExample.Add("Holden", 200);_ is used to add a key-value pair to the dictionary.

_dictionaryExample.Remove("BMW");_ is used to remove a key-value pair.

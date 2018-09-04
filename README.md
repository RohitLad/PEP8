# PEP8 guidelines

## Python Enhancement Proposals

## Recommendations:

- Use spaces instead of tabs
- Use 4 spaces for intendation
- Limit each line to a maximum of 79 characters, this helps with code readibility

## Imports

- Be as specific as possible with imports
``` python
# Do
from time import time
# Or
import time
# instead of
from time import *
```

- Split imports with the following priority
  1. Standard python libraries
  2. Third party libraries
  3. Application / library specific
``` python
# stdlib
import time
# Third party
import numpy
# Modules
from config import ...
...
```

## Commenting

- Bad comments are worse than no comments
- Use docstrings instead for auto-documentation
``` python
"""A docstring is a string that appears as the first statement in a module, function or a class

Multi-line docstrings consists of a summary line just like one lined docstring

Followed by a blank line and a more elaborate description
"""
```

## Naming

- Use ```CapWords``` for class names
- Use ```lowercase_with_underscores``` for Method, functions and variables
- Private methods and properties start with a ```__double_underscore```
- Use ```self``` as the first argument to instance methods
- Use ```cls``` as the first argument to class methods
- Never declare lambda functions ```f = lambda x: x**2```

``` python
class SomeClass:
    """This is an illustrative class"""
    
    __property = None
    
    def __init__(self, prop_value):
        self.__property = prop_value
        
    def get_property(self):
        """ A simple method to get property"""
        
        return self.__property
    
    @classmethod
    def default(cls)
        instance = MyClass("default value")
        return instance
```

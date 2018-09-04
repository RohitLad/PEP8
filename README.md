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

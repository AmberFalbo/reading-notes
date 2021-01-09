# 401 Notes-09: Game of Greed 4 (Magic, Special Methods)
[Back to 401 Index](401-index.md)<br>

## [Dunder Methods](https://dbader.org/blog/python-dunder-methods)
We are already a bit familiar with Dunder Methods as
```
__init__ or __str__
```
You can also use a dunder to emulate behavior of built-in types.
This is with using len as you usually couldn't use it in an empty class.
```
class LenSupport:
    def __len__(self):
        return 42

>>> obj = LenSupport()
>>> len(obj)
42
```

#### Another example is slicing. You can implement a __getitem__ method which allows you to use Python's list slicing syntax:obj[start:stop]


### Object Initialization: __init__
Right upon starting my class I already need a special method. To construct account objects from the Account class I need a constructor which in Python is the __init__ dunder:
```
class Account:
    """A simple account class"""

    def __init__(self, owner, amount=0):
        """
        This is the constructor that lets us create
        objects from this class
        """
        self.owner = owner
        self.amount = amount
        self._transactions = []
```

## [Statistics - Probability]()


## [Into to Statistics]()



## [AI Guru makes $238,800 with misleading paid course. doesn’t credit developers]()


## [Statistics Module]()




<!-- notes here -->


[Back to 401 Index](401-index.md)
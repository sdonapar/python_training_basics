# [Python](https://www.python.org) - Classes

* ## Python classes provide all the standard features of Object Oriented Programming
* ## The class inheritance mechanism allows multiple base classes
* ## A derived class can override any methods of its base class or classes

``` python
# simple class
class MyClass:
    """This is a sample class"""
    class_variable = 1.2
    def __init__(self,name):
        self.name = name
    def get_name(self):
        return self.name
    def set_name(self,name):
        self.name = name
```

``` python
print(MyClass.class_variable)
myobj = MyClass('My Object')
print(myobj.class_variable)
print(myobj)
print(type(myobj))
print(myobj.get_name())
myobj.set_name()
print(myobj_get_name())
```

``` python
# Class inheritance
class MyNewClass(MyClass):
    def __init__(self,name,age):
        super().__init__(name)
        self.age = age
```

``` python
newobj = MyNewClass("Test",30)
newobj.age
```

## Modules

* ## A module is a file containing Python definitions and statements. The file name is the module name with the suffix .py appended.
* ## Reuse of code
* ## Modularity for maintenance of the code base

* ## let's check what is there in [utilities.py](utilities.py) file
* ## the module name is "utilities"

``` python
import utilities
print(dir(utilities))

# accessing the functions in utilities module
utilities.hello("yourname")
```

# [Packages](./images/fig_packages.png)

* ## Packages are a way of structuring Python’s module namespace

* ### Suppose you are creating a software package for restaurant business
* ### Think, How you want to oganize your code
* ### What are the various functions necessary
* ### booking
* ### billing
* ### discounts
* ### menu

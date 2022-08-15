## [Python](https://www.python.org) - Basic Data Types

### Python is dynamically typed language
### Dynamically typed programming languages do type checking at run-time as opposed to Compile-time. 

``` python
iam_integer = 100
iam_float = 3.14
iam_str = "Hellow"
iam_bool = True
iam_complex = 3+4j
```

### Everything in Python is an object
### Everything in Python has a type
### **type** and **object** are special objects in python

``` python
print(type(iam_integer))
print(type(iam_float))
print(type(iam_str))
print(type(iam_bool))
print(type(iam_complex))
```

### What Are [Namespaces](./images/namespace.jpg) In Python?
* #### A namespace is a simple system to control the names in a program. It ensures that names are unique and won’t lead to any conflict.
### Local Namespace
* #### This namespace covers the local names inside a function. Python creates this namespace for every function called in a program. It remains active until the function returns.
### Global Namespace
* #### This namespace covers the names from various imported modules used in a project. Python creates this namespace for every module included in your program. It’ll last until the program ends.
### Built-in Namespace
* #### This namespace covers the built-in functions and built-in exception names. Python creates it as the interpreter starts and keeps it until you exit.


### Strings ( Immutable )


### List ( Mutable)
### Dictionary ( Mutable )
### Set ( Mutable )
### Tuple ( Immutable )
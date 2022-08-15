# [Python](https://www.python.org) - Functions

* ## The keyword **def** introduces a function definition.
* ## The **first statement** of the function body can optionally be a string literal
* ## This string literal is the function’s documentation string, or **docstring**.
* ## Variable Scope - local, global and then builtin
* ## Default Argument Values
* ## Keyword Arguments
* ## \*args and \**kwargs


## it is always a good practice to provide the docstring

``` python
# simple function without any return value

def simple_function():
    """This is a simple functions without any arguments"""
    print("This is a simple function")
```

``` python
# getting help and executing the function

help(simple_function)
simple_function()
```

``` python
# function with arguments

def squares(a):
    """This function returns the square of a given number
       squares(number) -> square of the number"""
    return a*a
```

``` python
# Providing a default value
# 
def squares(a=2):
    """This function returns the square of a given number
       squares(number=2) -> square of the number"""
    return a*a
```

``` python
def send_email(to="no_email",subject="No Subject",from_add="Sasi@example.com",body="no_content"):
    return "To:" + to + ";\nSubject:" + subject +";\nFrom:" + from_add + ";\nbody:" + body + "\n"
```

``` python
send_email(to="unknown@example.com",subject="This is a test message",body="I am in Python training")
```
## Function scope

``` python
a = 15
def myfunc(b):
    print('a:',a)
    return a + b

myfunc(3)
myfunc(5)
```

``` python
def newfunc(b):
    a = 5
    print('a:', a)
    return a + b

print('global a:', a)

newfunc(5)
newfunc(3)

print('global a:', a)
```

``` python
def globfunc(b):
    global a
    a = 5
    print('a:', a)
    return a + b

globfunc(7)
print('global a:', a)
```

## \*args and \**kwargs

``` python
def test_args(*args,**kwargs):
    for arg in args:
        print(arg)
    for key in kwargs:
        print(key,kwargs[key])

test_args(1,3,4,language='Python')

input_list = ['a','b','c','d']
input_kwargs = {'language':'Python'}
test_args(*input_list,**input_kwargs)
```


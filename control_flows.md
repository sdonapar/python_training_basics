# [Python](https://www.python.org) - Control Flows

``` python
# variable assignment
a = 10

a,b = 10,15
a,b

#swapping numbers
a,b = b, a
a,b

my_list = []
my_list = 12,18
my_list
```

``` python
# operatos - == < > <= >= n
age = 30
print(age == 30)
print(age <= 30)
print(age < 30)
print(age > 30)
print(age >= 30)
print(age != 30)
```

``` python
# if conditional statement
my_age = int(input("Enter Your age: "))

if (my_age <= 35):
    print("Young, consider investing in equities")
elif((my_age > 35) and (my_age <= 50)):
    print("Middle age , consider moving to secure instruments")
elif((my_age > 50) and (my_age <= 65)):
    print("You probably might be thiking of retiring now")
else:
     print("Might have retired already!!")
```

``` python
# comparing lists

my_list1 = [2,3,4]
my_list2 = [3,2,4]
my_list3 = [1,2,3]

print(my_list1 == my_list2)

print(my_list1 == sorted(my_list2))

print(my_list3 < my_list1)
```

``` python
# for loop
# iterates over the items of any sequence (list, string, tuple,dictinary,set)

number_list = range(1,10)

# find all of the odd numbers between 1 and 10
# 0 is False and >0 is True

for number in number_list:
    if (number%2):
        print(number)

```



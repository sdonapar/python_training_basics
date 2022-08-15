# [Python](https://www.python.org) - Functions

# Reading and writing Files

``` python
# open file for writing # w, wb

file_handle = open('output.txt','w')
print(file_handle)

# writing some data to file

file_handle.write("This is first line\n")
file_handle.write("This is second line\n")

# closing file handle
file_handle.close()
```

``` python
# opening file for reading
inp_file = open('output.txt','r')

for line in inp_file:
    print(line.strip("\n"))

# closing file handle
inp_file.close()
```

``` python
# with takes care of opening and closing the files, there is no explict closing is required
with open('output.txt','r') as f:
    print(f.read())
```
``` python

data = []
with open('output.txt') as f:
    data = f.readlines()

print(data)
```

``` python
# reading and writing data using pathlib

from pathlib import Path
# read_text, read_bytes
# write_text, write_bytes

data = """
This is first line
This is second line
"""

file_size = Path("output1.txt").write_text(data)
print(file_size)

file_data = Path("output1.txt").read_text()

print(file_data)
```

# Script explicado RedPanda 

## Import os

> The OS module in Python provides functions for interacting with the operating system. OS comes under Python’s standard utility modules. This module provides a portable way of using operating system-dependent functionality. The *os* and *os.path* modules include many functions to interact with the file system

```
os.name
#output 
posix
```

## Import requests

> allows you to send HTTP/1.1 requests extremely easily. There’s no need to manually add query strings to your URLs, or to form-encode your POST data. Keep-alive and HTTP connection pooling are 100% automatic, thanks to urllib3.


# Import sys 

> The sys module in Python provides various functions and variables that are used to manipulate different parts of the Python runtime environment. It allows operating on the interpreter as it provides access to the variables and functions that interact strongly with the interpreter. Let’s consider the below example.


Un ejemplo de esto es la manipulacion de argumentos que se le pasan al script ejemplo:

```
./script.py Hello Python agr3 masa
#out 
['./script.py', 'Hello', 'Python', 'agr3', 'masa']

sys.argv[0] == ‘script.py’ 
sys.argv[1] == ‘Hello’ 
sys.argv[2] == ‘Python

```


















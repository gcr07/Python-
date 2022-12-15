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

## Import  pdb — The Python Debugger

> The module pdb defines an interactive source code debugger for Python programs. It supports setting (conditional) breakpoints and single stepping at the source line level, inspection of stack frames, source code listing, and evaluation of arbitrary Python code in the context of any stack frame. It also supports post-mortem debugging and can be called under program control.

### Break point

```
pdb.set_trace()
```
te aparece un prompt ahi puedes poner por el nombre de la variable por ejemplo en el caso del script pues "command" ademas si pones la "l" te pone en que linea.

![image](https://user-images.githubusercontent.com/63270579/207769257-945472c3-9b7a-4b1c-8e51-e7ac5a5aa7b9.png)


## SIGNAL in Linux

> A signal is an event generated by the UNIX and Linux systems in response to some condition. Upon receipt of a signal, a process may take action. A signal is just like an interrupt; when it is generated at the user level, a call is made to the kernel of the OS, which then acts accordingly.

```
man signals

```

![image](https://user-images.githubusercontent.com/63270579/207737677-f2118d2d-944c-4561-9bcb-cfae917124a4.png)


## Import signal

> Este módulo proporciona mecanismos para usar gestores de señales en Python.

> La función signal.signal() permite definir gestores personalizados que serán ejecutados cuando una señal es recibida. Un pequeño número de gestores por defecto son instalados: SIGPIPE es ignorada (por lo que los errores de escritura en tuberías y sockets se pueden informar como excepciones ordinarias de Python) y SIGINT es trasladada en una excepción KeyboardInterrupt si el proceso padre no lo ha cambiado.

```

def def_handler(sig, frame):
	print("\n\n [!] Saliendo...\n")
	sys.exit(1)

signal.signal(signal.SIGINT, def_handler)

```


## Import time

> This module provides various time-related functions. For related functionality, see also the datetime and calendar modules.

Por ejemplo se puede usar sleep:

```
#!/usr/bin/python3 

import requests,sys,pdb,signal,os, time 


def def_handler(sig, frame):
	print("\n\n [!] Saliendo...\n")
	sys.exit(1)

signal.signal(signal.SIGINT, def_handler)

if __name__ == '__main__':
	time.sleep(10)

```


## Python ord()

> The ord() function returns an integer representing the Unicode character.

```
print(ord('@'))   
64
>>> print(ord('A'))                    
65   

```










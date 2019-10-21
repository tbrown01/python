# Python 2.7 Basics For Linux Systems Administrators
**SHA-BANG** The sha-bang (#!) at the head of a script tells your system that this file is a set of commands to be fed to the command interpreter indicated. Set the file permissions to be executable and then run the script.
```
~]$ vim python_script.py

#!/bin/python

print("Hello, World!")
wq!

~]$ chmod u+x python_script.py
~]$ ./python_script.py
Hello, World!
```

**Read Evaluate Print Loop (REPL)** is an environment that Python provides to experiment with Python code.

```
~]$ python
Python 2.7.5 (default, Aug  7 2019, 00:51:29) 
[GCC 4.8.5 20150623 (Red Hat 4.8.5-39)] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> exit()
~]$ 
```

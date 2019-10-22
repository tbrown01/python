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
## Data Types - Strings and Numbers

Python has five standard Data Types:

- Strings
- Numbers
- Lists
- Tuples
- Dictionary

## Strings
Create string variables by enclosing characters in quotes. Python uses single quotes ' double quotes " and triple quotes """ to denote literal strings. Only the triple quoted strings """ also will automatically continue across the end of line statement.

```
firstName = 'john'
lastName = "smith"
message = """This is a string that will span across multiple lines. Using newline characters
and no spaces for the next lines. The end of lines within this string also count as a newline when printed"""
```
Strings can be accessed as a whole string, or a substring of the complete variable using brackets ‘[]’. Examples:
```
var1 = 'Hello World!'
var2 = 'RhinoPython'

print var1[0] # this will print the first character in the string an `H`
print var2[1:5] # this will print the substring 'hinoP`
```
Python can use a special syntax to format multiple strings and numbers. The string formatter is quickly covered here because it is seen often and it is important to recognize the syntax.
```
print "The item {} is repeated {} times".format(element,count))
```
Python has a set of **built-in methods** that you can use on strings. **Note:** All string methods returns new values. They do not change the original string. Examples:

**lower()** method returns the string in lower case

**upper()** method returns the string in upper case

**replace()** method replaces a string with another string

```
abc = "Hello, World!"

print(abc.upper())            # Outcome Variable abc will be: HELLO, WORLD!

print(abc.lower())            # Outcome Variable abc will be: HELLO, WORLD!

print(abc.replace("H", "J"))  # Outcome Variable abc will be: JELLO,WORLD!
```
## Numbers

Python numbers variables are created by the standard Python method:
```
var = 382
```
Most of the time using the standard Python number type is fine. Python will automatically convert a number from one type to another if it needs. But, under certain circumstances that a specific number type is needed (ie. complex, hexidecimal), the format can be forced into a format by using additional syntax in the table below:

| Type | Format | Description |
| ------------- | ------------- |
| int  | a = 10 | Single Integer |
| float  | a = 45.67 | . Floating Point Real Values |
| long | a = 345L  | Can be Represented in Otcal & Hexadecimal |
| complex | a = 3.14j | (J) Contains Integer in Range of 0 to 255 |
 	  	  	  	  	  	 
Most of the time Python will do variable conversion automatically. You can also use Python conversion functions (int(), long(), float(), complex()) to convert data from one type to another. In addition, the type function returns information about how your data is stored within a variable.
```
message = "Good morning"
num = 85
pi = 3.14159

print(type(message))  # This will return a string
print(type(n))  # This will return an integer
print(type(pi))  # This will return a float
```

# 401 Notes-03:
[Back to 401 Index](401-index.md)<br>



## Reading and Writing Files in Python (Guide)

### What is a file?
At its core, a file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.

```
Files on most modern file systems are composed of three main parts:
	1.	Header: metadata about the contents of the file (file name, size, type, and so on)
	2.	Data: contents of the file as written by the creator or editor
	3.	End of file (EOF): special character that indicates the end of the file
```
What this data represents depends on the format specification used, which is typically represented by an extension. For example, a file that has an extension of .gif most likely conforms to the Graphics Interchange Format specification. There are hundreds, if not thousands, of file extensions out there. For this tutorial, you’ll only deal with .txt or .csv file extensions.

### File Paths
```
When you access a file on an operating system, a file path is required. The file path is a string that represents the location of a file. It’s broken up into three major parts:
	1.	Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)
	2.	File Name: the actual name of the file
	3.	Extension: the end of the file path pre-pended with a period (.) used to indicate the file type
```
```
Character
Meaning
'r'
Open for reading (default)
'w'
Open for writing, truncating (overwriting) the file first
'rb' or 'wb'
Open in binary mode (read/write using byte data)
```

## Python Exceptions: An Introduction

### Exceptions versus Syntax Errors
- syntax errors occur when the parser detects and incorrect statement. 
- exception error occurs whenever syntactically correct Python code results in an error. 

### Raising an Exception
- we can use “raise” to throw an exception if a condition occurs. The statement can be complemented with a custom exception. 

### The AssertionError Exception
- Instead of waiting for a program to crash midway, you can also start by making an assertion in Python. We assert that a certain condition is met. If this condition turns out to be True, then that is excellent! The program can continue. If the condition turns out to be False, you can have the program throw an AssertionError exception.

###The try and except Block: Handling Exceptions
- The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. 




## Reading and Writing Files in Python Videos

### opening and closing files in Python

Files can be opened with the “open” statement:
` file = open(“text_file.txt”) `
Files should always be closed after use, using “close”:
` file = close() `

To ensure file closes no matter if errors occur:

Using a try: finally: block:
```
file = open(“text_file.txt”)
try:
    # processing of data here
finally:
    file.close()
```
Using with:
```
with open(“text_file.txt”) as file:
    # processing of data here

# file is automatically closed at this point
```
(these following are locked)
- reading from a file
- writing to a file
- appending to a file
- file locations and paths
- what is a file?
- examining the contents of some files types



[Back to 401 Index](401-index.md)
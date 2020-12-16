# 401 Notes-04:Objects, Classes, Recursion & Pytest
[Back to 401 Index](401-index.md)<br>


## [Classes and Objects](https://www.learnpython.org/en/Classes_and_Objects)

### Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.

Basic class:
```
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")
```

Assigning a class(template) to an object.
```
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()
```

### Accessing Object Variables
To access a variable out the newly created "myobjectx":
```
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()

myobjectx.variable
```

### Accessing Object Functions
To access a function inside of an object you use notation similar to accessing a variable:
```
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()

myobjectx.function()
```







## [Thinking Recursively](https://realpython.com/python-thinking-recursively/)

![Thinking Recursively](../assets/Thinking-Recursively.jpg)


## [Pytest Fixtures and Coverage](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)

In pytest, you define fixtures using a combination of the pytest.fixture decorator, along with a function definition. For example, say you have a file that returns a list of lines from a file, in which each line is reversed:

```
def reverse_lines(f):
   return [one_line.rstrip()[::-1] + '\n'
           for one_line in f]

```


## [Pytest Fixtures](https://docs.pytest.org/en/latest/fixture.html)

```
capfd
Capture, as text, output to file descriptors 1 and 2.

capfdbinary
Capture, as bytes, output to file descriptors 1 and 2.

caplog
Control logging and access log entries.

capsys
Capture, as text, output to sys.stdout and sys.stderr.

capsysbinary
Capture, as bytes, output to sys.stdout and sys.stderr.

cache
Store and retrieve values across pytest runs.

doctest_namespace
Provide a dict injected into the docstests namespace.

monkeypatch
Temporarily modify classes, functions, dictionaries, os.environ, and other objects.

pytestconfig
Access to configuration values, pluginmanager and plugin hooks.

record_property
Add extra properties to the test.

record_testsuite_property
Add extra properties to the test suite.

recwarn
Record warnings emitted by test functions.

request
Provide information on the executing test function.

testdir
Provide a temporary test directory to aid in running, and testing, pytest plugins.

tmp_path
Provide a pathlib.Path object to a temporary directory which is unique to each test function.

tmp_path_factory
Make session-scoped temporary directories and return pathlib.Path objects.

tmpdir
Provide a py.path.local object to a temporary directory which is unique to each test function; replaced by tmp_path.

tmpdir_factory
Make session-scoped temporary directories and return py.path.local objects; replaced by tmp_path_factory.
```






[Back to 401 Index](401-index.md)
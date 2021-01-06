# 401 Notes-07: Game of Greed 2
[Back to 401 Index](401-index.md)<br>




## Python Scope & the LEGB Rule: Resolving Names in Your Code

### Understanding Scope
In programming, the scope of a name defines the area of a program in which you can unambiguously access that name, such as variables, functions, objects, and so on. A name will only be visible to and accessible by the code in its scope. Several programming languages take advantage of scope for avoiding name collisions and unpredictable behaviors. Most commonly, you’ll distinguish two general scopes:

<b>Global scope:</b> The names that you define in this scope are available to all your code.

<b>Local scope:</b> The names that you define in this scope are only available or visible to the code within the scope.





```
Operation	Statement
Assignments	x = value
Import operations	import module or from module import name
Function definitions	def my_func(): ...
Argument definitions in the context of functions	def my_func(arg1, arg2,... argN): ...
Class definitions	class MyClass: ...

```

### Using the LEGB Rule for Python Scope
Python resolves names using the so-called LEGB rule, which is named after the Python scope for names. The letters in LEGB stand for Local, Enclosing, Global, and Built-in. Here’s a quick overview of what these terms mean:

Local (or function) scope is the code block or body of any Python function or lambda expression. This Python scope contains the names that you define inside the function. These names will only be visible from the code of the function. It’s created at function call, not at function definition, so you’ll have as many different local scopes as function calls. This is true even if you call the same function multiple times, or recursively. Each call will result in a new local scope being created.

Enclosing (or nonlocal) scope is a special scope that only exists for nested functions. If the local scope is an inner or nested function, then the enclosing scope is the scope of the outer or enclosing function. This scope contains the names that you define in the enclosing function. The names in the enclosing scope are visible from the code of the inner and enclosing functions.

Global (or module) scope is the top-most scope in a Python program, script, or module. This Python scope contains all of the names that you define at the top level of a program or a module. Names in this Python scope are visible from everywhere in your code.

Built-in scope is a special Python scope that’s created or loaded whenever you run a script or open an interactive session. This scope contains names such as keywords, functions, exceptions, and other attributes that are built into Python. Names in this Python scope are also available from everywhere in your code. It’s automatically loaded by Python when you run a program or script.

## Basic Programming With Python


### Loops
There are two different kinds of loops in Python: the for loop and the while loop.

### The For Loop
The for loop iterates over a list, or an array, of objects. You have probably seen this code before:


### The While Loop
While loops don't loop over a list. They loop over and over and over...until...a condition becomes false.






[Back to 401 Index](401-index.md)
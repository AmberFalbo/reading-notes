[Main](https://amberfalbo.github.io/learning-journal/)

~~***Rememeber***~~
```
MVC - Minimum Viable Code - remember not to over do it!
Leave comment in code for myself!
“ command / “  
also make a todo list, todo tree  // TODO: “add something”
paste the reqs right in the code so you know what to do THEN work on the fun stuff!
```

# Programming with JavaScript
### class 07

we learned conditionals yesterday

## today is **functions**

>"Write out things 5 times on paper and 5 times on the computer!!"

### 4 foundational pieces for JS
- function 
- loops
- arrays
- conditionals

# Programming 

How is programming like baking a cake.
- the right ingredients
- in the right orders

Coding is telling the computer what you want it to do, only what you tell it to do!

```
**How to tell a Robot how to put on a sweater that has a hood to put on and a zipper that is already zipped up.
- pick up the sweater
- hold sweater with one hand
- grab pull tab of the zipper
- pull the pull tab of the zipper down until it unhooks
- hold the sweater in a way where the hood is topside
- adjust the sweater so that it is open to your back from the inside 
- move the sweater so that the left arm can slide into the left sleeve 
- insert left arm into left sleeve 
- move right shoulder to adjust so that the right arm can slip into right sleeve
- insert right arm into right sleeve 
- adjust sweater to close in the front 
- grab zipper and connect to the other zipper part on the other side
- pull up on the zipper while pulling down the bottom of the sweat with other hand
- pull all the way up to the top of the sweater
- reach back to behind the head
- grab the hood
- pull the hood up and over to fit on head
**this is how easy it is to break code!**
```
Work for
read 07

>Reference
Duckett: JavaScript & jQuery:
Intro + Scripts: Pages 1 - 24
Expressions + Operators: 74 - 79
Functions: 88 - 94. (focus on this the most!!!)



## **Vocab**
- Script - 
- JavaScript's vocabulary - 
- JavaScript's syntax - 
- Programmatic problem solving - 
- Expression
- Operator
- Function - **from the review** ***A reusable set of step-by-step instructions, potentially based on input, to potentiallly provide some outputs.***  Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements). *Furthermore the statements in a function are not always executed when a page loads, so functions also offer a way to  **store** the steps needed to achieve a task.* ***for example, you might have a task that you only want to perform iff the user clicks on a specific element in the page.***
  - Declaration - The variable is registered using a given name within the corresponding scope.
  - Call - the call () allows for a function/method belonging to one object to be assigned and called for a different object. **call** () provides a new value of this to the function/method. With **call** (), you can write a method once and then inherit it in another object, without having to rewrite the method for the new object. *naming a function to perform a task so you make call on it later* 
  - Parameters - some functions need to be provided with information in order to achieve a given task. *for example, a function to calculate the area of a box would need to know its width and height. **Pieces of information passed to a function are known as parameters.**
  - Arguments
  - Return value - When you write a function and you expect it to provide you with can answer, the response is known as a **return value**.
- Refactoring

## To create a function, you give it a name and then write the statements needed to achieve its task inside the curly braces.
### This is known as a **function declaration**
- You declare a **function** using the **function** keyword.
You give the function a **name** (sometimes called an **identifier**) followed by parenthesis. 
- The **statement** that perform the task sit in a code block. (They are inside curly braces.)

```
function say Hello() {
	document.write(‘Hello!’);
}
```

#JavaScript

## Demo: Functions

**don’t use document.write()** in 201
*someone could take over your code*

```
‘use strict’; - makes js evaluate your code stronger

console.log(‘im alive’);  - just prints that over to console

var userName = prompt (‘what is your sith name’) ; - assigning name

var isSithLordOrMaster = probt (;are you a sith lord?’).toUpperCase(); = prompt to response, change with upper or lower case

if (isisthlordOrmaster === ‘no’ = if you entered sith or lord then t
```

**part of class 07 check the recording for reminders!**

## function syntax example

```
function askNEwSithQuestion() {
	var NewQuestion = promt(‘can you beat master yoda’;
	console.log(newQuestion);
}
```
**also curly can go inside curly**

## why doesn’t it work? haven’t called/evoked the function yet

```
askNewSithQuestion();

```

()= envoking/calling method or function
**always remember to invoke function**

# functions are for reusability and organization!
## wrap code in functions!!	

### Add function ex

```
function add(a,b) {
	console.log(a +b);
	return a + b;
}
```
**return helps you send something out of your function**
once a function sees a return it stops and moves on, nothing can be under the return
### the invocation

```
var fivePlusTen = add(5,10);
add(110,34);
add(45,45);

```
**rember console log is just shown in console - just printing it to the console

you need to declare a variable to save the return function on the invocation
- var = stores it


var names = makes sense to what you are asking

function names = name apply to what it’s doing
or 

```
var c = 10;
var fivePlusTen = add(5,10);
add(c,34);
add(45,45);

```
“ var c “ - global variable

# order matters!

# what happens in the function stays in the function

or if
 you did 
add(‘c’ + 34)

= c34 
‘’ - cancatenator 

Need to enter in strings

# JavaScript executes **top to bottom**

global var = username, c 
local var = a or b

function invoking= ldkfjdljfd();

Global variables are defined outside of function. Local variables are defined inside of a function and only lives within the function.

Function invocation is the function name and then parentheses.
So like functionName();

If your function has parameters, like Roger’s add function, then you also pass arguments to the parameters in the parentheses.

the invocations- control order of operations

## review again of functions!

## 2 things to do with functions
- declare it 
- invoke it

## functions
- accepts/takes perarmeters

## when invoking functionsit is an argument
- they will map to perameters inside function 




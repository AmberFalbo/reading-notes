# Class 04 - April 30th, 2020
[Back to 201 Index](./../201-index.md)<br>
## Morrning
Code Review!!

the ‘ . ‘ in vscode indicates that they are hidden files from git!

add directions in the read.me

there is a eslint for .md in the repo! 

Eslint = guidelines to follow/rules add to file when writing to code and works like a spell checker

- companies often has their own guidelines

The README.md - for when people look at your code
- how would I run this application
- notes on what this app does
- why did I make this app.
- “I made this so you would get to know me”
*look at other read.me files*

parseInt(); 
Number();

these above help change a string into a number

console.log(parseInt('4'));

console.log(Number('4'));

4 + "";


add semi colons ; always as the end of variations, it means end of sentence

== truthy

=== strict equal

for(var i = 0; i<6; i++){
  //do sometthhing
}

if (conditiong){
  // dosomething
}

if(conditon){
  // do something
} else if(condition){
  // do somethhing
} else if(condition){
  // do something 
}




# Data Types in javaScrip

1. String - anything that you put in quotes

2. Numbers - nmber (2, 5, -4, 782)

3. Boolean - true or false

4. Object - save for late


Truthy and Falsy
* things that are falsy
	1. 0
	2. false
	3. “” (if empty)
	4. null
	5. undifined
	6. Nan

```

if('I am string'){console.log('this is a truthy statement')} else{('this is a false statement')}
VM367:1 this is a truthy statement
undefined

if(''){console.log('this is a truthy statement')} else{('this is a false statement')}
"this is a false statement"

if(12){console.log('this is a truthy statement')} else{('this is a false statement')}
VM392:1 this is a truthy statement
undefined

if(0){console.log('this is a truthy statement')} else{('this is a false statement')}
"this is a false statement"

if(undefined){console.log('this is a truthy statement')} else{('this is a false statement')}
"this is a false statement"

```

practice from lab

```
2 ===2
true
2=='2'
true
2 === '2'
false

```

## parseInt examples

```
var stringTwo = '2';
undefined
parseInt(stringTwo)
2
```
```
var intTwo = parseInt(stringTwo)
undefined
intTwo === 2
true
```
```
2 ===parseInt('2')
true
```
```
2 === parseInt(stringTwo)
true
```

typeof = tells you what type of data type

```
typeof stringTwo
"string"

typeof intTwo
"number

```


# functions!!

// top bun
function userResponse(){
var userAnswer = 'yes';

  //if statement

  if(userAnswer === 'yes'){
    console.log('the user answered yes');
  } else {
    console.log('the user did not answer yes');
  }
}


You need to grab the statement and put it inside the function then call it by name! 

invoking the function

// in order for a funtion to run, you have to call it by name, We call this invoking the function
userResponse();


```
// top bun
function userResponse(){
  // this variable is SCOPED to this function, It is NOT accessible outsie of this function.
  var userAnswer = 'yes';

  //if statement

  if(userAnswer === 'yes'){
    console.log('the user answered yes');
  } else {
    console.log('the user did not answer yes');
  }

  console.log('the userAnswer is  ' + userAnswer);
}

// in order for a funtion to run, you have to call it by name, We call this invoking the function
userResponse();

```

Putting a function in your function!

```

// top bun
function userResponse(){
  // this variable is SCOPED to this function, It is NOT accessible outsie of this function.
  var userAnswer = 'yes';

  //if statement

  if(userAnswer === 'yes'){
    sayYes();
  } else {
    console.log('the user did not answer yes');
  }

  console.log('the userAnswer is  ' + userAnswer);
}

function sayYes(){
  console.log('the user answered yes');
}



// in order for a funtion to run, you have to call it by name, We call this invoking the function
userResponse();

```

You can have as many functions as you want in your function

ig

```
function getAllData(){
  getUserINfo();
  getAddress();
  getPhone();
  getFriendList();
}

```

# perameters

the parameter
```
function greeting(message){
  console.log(message);
}

```

the argument 
```
greeting('hello everyone');

```


you can change your argument but you wont change the parameter (message)
argument = what the user says

you can have one parameter

```
  if(userAnswer === 'yes'){
    greeting('howdy', '201 class');
  } else {
    console.log('the user did not answer yes');
  }

  console.log('the userAnswer is  ' + userAnswer);
}

function greeting(message, className){
  console.log(message);
  console.log(className);
}
```

setting defaults

```
  if(userAnswer === 'yes'){
    greeting();
  } else {
    console.log('the user did not answer yes');
  }

  console.log('the userAnswer is  ' + userAnswer);
}

function greeting(message='hi', className='201'){
  console.log(message);
  console.log(className);
}
```


// parameter: a variable that a function takes in and can use.

// argument: the actual thing i give the function when i call it that fees the parameter

need a return
```
function numberSum(num1, num2){
  var sum = num1 + num2;
  return sum;
}

numberSum(4,5);

```

# CSS

```
div{
  border: 1px solid red;
  padding: 20px;
  margin: 10px;
  width: 40px;
  position: static;
}

section{
  height: 1000px;
}

/* completely out of the flow of the document */
#absolute{
  position: absolute;
  top: 40px;
  left: 200px;
  background-color: green;
  color: white;
}

/*  pays attention to flow of the document */
#relative{
  position: relative;
  top: 40px;
  left: 200px;
  background-color: cyan;
}

#fixed{
  position: fixed;
  background-color: purple;
  color: white;
  left: 300px;
  top: 40px;
}

```
what the html looks like for the above

```
<section>
<div id="absolute"> box 1</div>
<div id="static"> box 2</div>
<div id="relative"> box 3</div>
<div id="fixed"> box 4</div>
<div> box 5</div>
</section>
```

# forking on github


Pair programming

partner sends you their github link

open partners github 
*fork (first!!!)
	this will add to your own github
*clone the new repo from partner (from your repo)
* add to terminal

*ACP often!!

*when done then ACP back up

new pull requst = asking partner if they can merge work back into theirs
 

** on your side when you get pull request**
* merge and confirm pull request


mkdir a directory for pair programming in 201

```
Pair Programing Steps
1. send your partner the link to your rep
2. your partner shoudl FORK your repo
3. your partner should clone your repo from his/her gitHub
4. your partner should open you repo from his/her local machine
5. PAIR PROGRAM
	- your are the navigator
	- your partner is the driver
6. your partner should A-C-P
regularily
7. when you are don(after 2 hours), your partner should make a pull request from his/her gitHub to your gitHub
8. accept the request in your gitHub and merge changes.

```

// upstream for changes but thats in 301




- I think it went really well for learning.
- Yes! Trevor helped me with cleaning up and organizing my arrays along with shortcuts to change the  names faster and more consice.
- I was nervous about getting to my project and worried it wouldn’t look at clean and organized for partner help.
- Communication was key and helped make this project go really smoothly!
- I took about an hour each which gave us time to do code review and work on stretch goals if we could fit them in and general spell checking and site errors.
- I thought this was going to take way longer like 3 hours each or at least a much longer time for me to navigate then it took!!


[Back to 201 Index](./../201-index.md)<br>



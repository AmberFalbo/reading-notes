# Class 05 - May 1st, 2020

## Code Review

### my about me
*add scrolling to my lists
	*make them next to each other
*look at courtneys wild cool funtions!!!
* make my food list links

Strings and Arrays have index postitions!

String
```
‘ y e s’
0 1 2
```
Array
```
‘yum, meow, cow’
0          1        2
```
# Order matters!!

## Global Variables
## Functions
## excutable/calling goes at very bottom

Deplay about me pages!!!

Talk about arrays!
 
to push on 

```
// Arrays

// push => add something to the end of an array 

var myFamily = ['Ilya', 'Adam', 'Tangerine', 'Maliki', 'Cookie'];

myFamily.push('ruby');

console.log(myFamily);
```

to push off
```

// pop => take the last thing off of an array

var myFamily = ['Ilya', 'Adam', 'Tangerine', 'Maliki', 'Cookie'];

myFamily.push('ruby');

myFamily.pop();

console.log(myFamily);

```

to add to the front of array (harder task)

```
// unshift => add something to the beginning of an array

var myFamily = ['Ilya', 'Adam', 'Tangerine', 'Maliki', 'Cookie'];

// myFamily.push('ruby');

// myFamily.pop();

myFamily.unshift('ruby');

console.log(myFamily);

```
() = function call 

array inside an array and anything

```
var myFamily = [
  'Ilya', 
  'Adam', 
  'Tangerine', 
  'Maliki',
  23,
  true, 
  'Cookie', ['spot', 'smalls', 'golden']
  ];
```

remove from first of list
```
// shift = remove the fist thing in the array

var myFamily = [
  'Ilya', 
  'Adam', 
  'Tangerine', 
  'Maliki',
  'Cookie',
  ];

myFamily.push('ruby');

myFamily.pop();

myFamily.unshift('ruby');

myFamily.shift();

console.log(myFamily);
```

indexOF
```
// indexOf => returns the index of an item in the array 

var myFamily = [
  'Ilya', 
  'Adam', 
  'Tangerine', 
  'Maliki',
  'Cookie',
  ];

// myFamily.push('ruby');

// myFamily.pop();

// myFamily.unshift('ruby');

// myFamily.shift();

// console.log(myFamily);

myFamily.indexOf('Adam');
```

splice

```

// splice => takes up to 3 arguments:
  // first: index position that you want to begin
  // second: how many items you want to remove (could be 0)
  // third: what you want to add (optional)

var myFamily = [
  'Ilya', 
  'Adam', 
  'Tangerine', 
  'Maliki',
  'Cookie',
  ];

myFamily.splice(1, 0, 'ruby');  

// myFamily.push('ruby');

// myFamily.pop();

// myFamily.unshift('ruby');

// myFamily.shift();

console.log(myFamily);
```
 can remove and addd
```
// splice => takes up to 3 arguments:
  // first: index position that you want to begin
  // second: how many items you want to remove (could be 0)
  // third: what you want to add (optional)

var myFamily = [
  'Ilya', 
  'Adam', 
  'Tangerine', 
  'Maliki',
  'Cookie',
  ];

myFamily.splice(1, 2, 'ruby');  

// myFamily.push('ruby');

// myFamily.pop();

// myFamily.unshift('ruby');

// myFamily.shift();

console.log(myFamily);

```

you don’t have to add in splice
```
var myFamily = [
  'Ilya', 
  'Adam', 
  'Tangerine', 
  'Maliki',
  'Cookie',
  ];

myFamily.splice(1);  

// myFamily.push('ruby');

// myFamily.pop();

// myFamily.unshift('ruby');

// myFamily.shift();

console.log(myFamily);

```

```
// returns removed items
```

challanges wh ita partner

challenge 1: put something in the middle of an array

```var myFamily = [
  'Ilya', 
  'Adam', 
  'Tangerine', 
  'Maliki',
  'Cookie',
  ];

myFamily.splice(2, 0,'ruby');  
```
10:33
challenge 2: remove two items from an array
```
var myFamily = [
  'Ilya', 
  'Adam', 
  'Tangerine', 
  'Maliki',
  'Cookie',
  ];

myFamily.splice(2, 2,'ruby');  
```
10:33
challenge 3: put three somethings in the middle of an array

```
var myFamily = [
  'Ilya', 
  'Adam', 
  'Tangerine', 
  'Maliki',
  'Cookie',
  ];

myFamilycice(1, 0, 'something', 'something1', 'somthing2');
```
10:33
challenge 4: write a function that takes in a name and a number and puts them both into an array and returns that array


```


```


Functions

return full name
```
function hello(firstName, lastName){
  var fullName = firstName + ' ' + lastName;
  return 'hello ' + fullName;
}

hello('bob', 'smith');

```

greeting too
```
function hello(firstName, lastName){
  var fullName = firstName + ' ' + lastName;
  var greeting = 'hello ' + fullName;

  return [fullName, greeting];
}

hello('bob', 'smith');

```

a function returning 2 arrays

```
function hello(firstName, lastName){
  var fullName = firstName + ' ' + lastName;
  var greeting = 'hello ' + fullName;

  return [fullName, greeting];
}

var greetingArray = hello('bob', 'smith');

console.log(greetingArray[0]);
```

```
bob smith
   
```

```
function hello(firstName, lastName){
  var fullName = firstName + ' ' + lastName;
  var greeting = 'hello ' + fullName;

  return [fullName, greeting];
}

var greetingArray = hello('bob', 'smith');

console.log(greetingArray[1]);
```

```
   
hello bob smith
   
```

Function Declaration
```
function hello(firstName, lastName){
  var fullName = firstName + ' ' + lastName;
  var greeting = 'hello ' + fullName;

  return [fullName, greeting];
}

var greetingArray = hello('bob', 'smith');

console.log(greetingArray[1]);
```

```
function sum (a, b){
  return a + b;
}

sum (4, 6);
```

```
// funtion declaration
  // you can call from anywhere
sum (4, 6);
function sum (a, b){
  return a + b;
}


// function expression


var sum = function (a, b){
  return a + b; 
}

sum (4, 6);
```

# google fonts



To embed a font, copy the code into the <head> of your html
<link> @import
<link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
CSS rules to specify families
	.	font-family: 'Pacifico', cursive;


LINKING

absolute link
```
<a href=“http://google.com”> google</a>
```

link to an id
```
<a href=“#travel”>Travel</a>
```

# DIG IN AND KNOW ABOUT ACCESSIBILITY!!!!
## learn about it, helps with getting a job!
sreen readers too

target makes you go to a knew page!

```
<a href=“#travel” taget=“_blank”> travel</a>
```

# branching!!

most important part of gitHub

<br>

```

1.
in Terminal
git checkout -b"name of branch"
ACP (while working)
git add .
git commit -m"message"
git push origin BRANCH NAME

2.
Go to gitHub
  Make a pull request from branch to master
  approve the merge

3.
in Terminal
git checkout master
git pull origin master

```








[Main](https://amberfalbo.github.io/learning-journal/)

# Operators and Loops
- learn how computers work, technical terminology, at more than one level of detail!
- learn how to implement `for` and `while` loops to accopli


## New Vocabulary

- loop - used to repeatedly run a block of code - until a certain condition is met.
- while - statement creates a loop that executes a block of code as long as the test condition evaluates to true . The while loop evaluates the expression before each iteration.
- for - to run code a specific number of times, use a for loop. The condition is usually a counter which is used to tell how many times the loop should run.
- condition - expression that evaluates whether something is true or false. When the value of a condition is true, we say that this condition is satisfied. 
- increment - `i++ or ++i`
- decrement - `i-- or --i`

 
### Reference
>Ducket: JavaScript & iQuery
Comparison and logical operators: 150-151, and 157
‘for’ and ‘while’ loops: 179-173, and 176


## Comparison and logical operators: Evaluating Conditions

You can evaluate a situation by comparing one value in the script to what you expect it might be. The result will be a Boolean: **true** or **false**.

`==` IS EQUAL TO

`!=` IS NOT EQUAL TO

`===` STRICTY EQUAL TO

`!==` STRICT NOT EQUAL TO

`>` GREATER THAN

`<` LESS THAN

`>=` GREATER THAN OR EQUAL TO

`<=` LESS THAN OR EQUAL TO


## Logical Operators
Comparison operators usually return single values of **true** or **false**. 
Logical operators allow you to compare the results of ore than one comparison operator.

**Do expression 1 and espression 2 both evaluate to true?**

**false**

`((5 < 2) && (2 >= 3))`

^Expression 1  ^Expression 2

**both are false**

`&&` LOGICAL AND

`||` LOGICAL OR

`!` LOGICAL NOT

## **Loops**
Loops check a condition. If it returns `true` , a code block will run. There are 3 common types of loops.

**For -  While -  Do While**

### **Condition**
Then the condition will be checked again and if it still returns true, the code block will rn again. It repeats until the condition returns false.

### **For Loop Example**
```
for (var i = 0; i < 10; i++) {
    document.write(i);
}
```


## **Loop Counters**

`var i = 0;` INITIALIZATION

`i < 10;` CONDITION

`i++` UPDATE

### **While Loop Example**
// = notes
```
var i = 1;  // set counter to 1
var msg = '';   // message

// store 5 times table in a variable
while (i < 10) {
    msg += i + ' x 5 = ' + (i * 5) + '<br /br>';
    i++;
}
```

***notes***

Array- great ex of a `for` loop

While loop needs a conditions
- going to run loop until number hits 50
- while number is less then 50 then run this loop
- when greater too or equal too then finish running loops




Run forever = infinite loop (overflow) ` i=

A for loop

```
For (var i = 0; I <=12; I = I +1) {
	console.log(I * 8);
}
```

## **DEMO on loops!**

```
'use strict';

var userName = prompt('What is your SITH name? (No Darth or Lord Titles)');
var isSithLordOrMaster = 'nope'


while( (isSithLordOrMaster != 'YES') && (isSithLordOrMaster != 'NO') ){
    isSithLordOrMaster = prompt('Are you a Sith Lord? (yes or no)').toUpperCase();
}

if(isSithLordOrMaster === 'NO'){
    var wannaBeSith = prompt('Are you aspiring to be a Sith?').toLowerCase();
}

function isTraining(){
    if (isSithLordOrMaster === 'YES'){
        alert('Welcome Darth ' + userName);
    }

    else if (wannaBeSith === 'no'){
        alert('Sith or Sith trainees only.  Beat it before I Force Choke you!!!');
        document.write('<h1>' + userName + 'Is About to get Force Choked!' + '<h1>');
    }
    else if (wannaBeSith === 'yes'){
        alert('Welcome to the Dark Side.  We have masks here!')
    }
}

function forceGuessingGame() {
 
    var correctAnswer = 32;

    for(var i = 0; i < 8; i = i + 1){
        var numberGuess = prompt('Please Guess a Number between 1 and 100');
        if(numberGuess == correctAnswer){
            alert('You are a true Sith Lord');
            break;
        } else {
            alert('Sorry, please try again!');
        }
        if (i == '7') {
            alert('You are no Sith!');
            isSithLordOrMaster = 'NO';
        }
    }
}

function darthFunction(){
    if(isSithLordOrMaster === 'YES'){
        document.write('<h1>' + 'Welcome Darth ' + userName + '! What is thy Bidding?' + '<h1>');
    }
}

function forceChoke() {
    if((isSithLordOrMaster === 'NO') && (wannaBeSith === 'yes')){
        document.write('<h3>' + 'The Dark Side of the Force is strong in ' + userName + '!' + '<h3>');
    }
}

isTraining();
forceGuessingGame();
darthFunction();
forceChoke();
```


Function forceGuessingGame()

**Lab 08**

1. Add validation on one of the user inputs.
- Keep asking until an acceptable value is entered. (While loop)

2. Guessing game!!  (Guessing game!) (for loop)



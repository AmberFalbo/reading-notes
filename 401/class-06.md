# 401 Notes-06: Game of Greed 1
[Back to 401 Index](401-index.md)<br>


## [How to use the Random Module in Python](https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)

### Randint
Use this when you want a randrom integer, Randit eccepts two parameters: a lowest and a highest number. Can generate integes between 1,5. The first value should be less than the scecond.

```
import random
print random.randint(0, 5)
```
This will output either 1, 2, 3, 4 or 5.

### Random
If you want a larger number, you can multipy it.

```
import random
random.random() * 100
```
### Choice
Generate a random value from the sequence sequence.
```
random.choice( ['red', 'black', 'green'] ).
```
The choice function can often be used for choosing a random element from a list.

```
import random
myList = [2, 109, False, 10, "Lorem", 482, "Ipsum"]
random.choice(myList)
```

### Shuffle

The shuffle function, shuffles the elements in list in place, so they are in a random order.

```
from random import shuffle
x = [[i] for i in range(10)]
shuffle(x)
```
### Randrange
Generate a randomly selected element 

```
from range(start, stop, step)
```

```
random.randrange(start, stop[, step])
import random
for i in range(3):
    print random.randrange(0, 101, 5)
```


## Why is Risk Analysis in Software Testing?


### Why use Risk Analysis?

After knowing about the risk areas, it helps the developers and managers to mitigate the risks. When a test plan has been created, risks involved in testing the product are to be taken into consideration along with the possibility of the damage they may cause to your software along with solutions.

Now, you might think what could be the possible risks that you could encounter? Well here is a list:

1. Use of new hardware
2. Use of new technology
3. Use of new automation tool
4. The sequence of code
5. Availability of test resources for the application

### Risk Identification

1. **Business Risks:** This risk is the most common risk associated with our topic. It is the risk that may come from your company or your customer, not from your project.

2. **Testing Risks:** You should be well acquainted with the platform you are working on, along with the software testing tools being used.

3. **Premature Release Risk:** a fair amount of knowledge to analyze the risk associated with releasing unsatisfactory or untested software is required

4. **Software Risks:** You should be well versed with the risks associated with the software development process.




[Back to 401 Index](401-index.md)
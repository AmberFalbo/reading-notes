# 401 Notes-01:
[Back to 401 Index](401-index.md)<br>

## [Pain and Suffering](https://codefellows.github.io/code-401-python-guide/curriculum/class-01/notes/pain_suffering)

### pain is growth

1. What’s your perspective? The greater the growth, the greater the pain.
1. Why are you doing this? to gain useful skills to become a Pythonista 
1. Do you want what comes at the end of this journey? to be financially independent. 
1. Are you doing this for you? Myself and for my family. 

## Big O

### [A beginner's guide to Big O notation](https://rob-bell.net/2009/06/a-beginners-guide-to-big-o-notation/)

### [A friendly intro to Big O Notation](https://www.codenewbie.org/basecs/8)

O(1) describes an algorithm that will always execute in the same time (or space) regardless of the size of the input data set.

```
bool IsFirstElementNull(IList<string> elements)
{
    return elements[0] == null;
}
```

O(N) describes an algorithm whose performance will grow linearly and in direct proportion to the size of the input data set. 

```
bool ContainsValue(IList<string> elements, string value)
{
    foreach (var element in elements)
    {
        if (element == value) return true;
    }

    return false;
}
```

O(N2) represents an algorithm whose performance is directly proportional to the square of the size of the input data set. This is common with algorithms that involve nested iterations over the data set. Deeper nested iterations will result in O(N3), O(N4) etc.

```
bool ContainsDuplicates(IList<string> elements)
{
    for (var outer = 0; outer < elements.Count; outer++)
    {
        for (var inner = 0; inner < elements.Count; inner++)
        {
            // Don't compare with self
            if (outer == inner) continue;

            if (elements[outer] == elements[inner]) return true;
        }
    }

    return false;
}
```

O(2N) denotes an algorithm whose growth doubles with each additon to the input data set. The growth curve of an O(2N) function is exponential - starting off very shallow, then rising meteorically. An example of an O(2N) function is the recursive calculation of Fibonacci numbers:

```
int Fibonacci(int number)
{
    if (number <= 1) return number;

    return Fibonacci(number - 2) + Fibonacci(number - 1);
}
```


## [Names and Values in Python](https://www.youtube.com/watch?v=_AEJHKGk9ns)
Python is simple
- works like other languages... until it doesn't 

- names refer to values
- many names can refer to one value
- names are reassigned independently 
- values live until no references
- assignment never copies data
- mutable aliasing
  - a mutable value
  - more than one name
  - the value changes
  - all names see the change!
- immutable values can't alias
  - immutable types: ints, floats, strings, tuples
- "change" is unclear
  - changing an int: rebinding
  - changing a list: mutating
  - can also rebind lists
  - can't mutate an int: ints are immutable
- Mutable and immutable are assigned the same
  - assignment is the same for <b>all</b> values
  - aliasing can make it seem different
- assignment variants
- references can be more than just names
  - list elements are references
- lots of things are references
  - object attributes
  - list elements
  - dict values (and keys!)
  - anything on the left side of an assignment

### [How to Setup an Awesome Python Environment for Data Science or Anything Else](https://towardsdatascience.com/how-to-setup-an-awesome-python-environment-for-data-science-or-anything-else-35d358cc95d5)



### [Python 3 Module of the Week](https://pymotw.com/3/index.html)


[Back to 401 Index](401-index.md)
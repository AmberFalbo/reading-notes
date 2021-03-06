# Read: 06 - JS Object Litrals; The Dom
[Back to 201 Index](201-index.md)<br>
### Readings:
**JavaScript & jQueary**
>Jon Duckett

- ch.3 - Object Literals (pp.100-105)
- ch.5 - Document Object Model (pp.183-242)

<br>

**Article**<br>
[Understanding the problem domain is the hardest part of programming.](https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming)

<br>

## **JavaScript & jQuery**

Chapter 3 - Object Literals (pp.100-105)
<br>
**Main Points**
- An object is a series of variables and functions that represent something from the world around you.
- In an object, variables are known as properties of the object; funtions are known as methods of the object.
- Web browsers implement objects that represent both the browswer window and the document loadded into the browser window.
- JavaScript also has several built-in objects suchas `String`, `Number`, Math`, and `Date`. Their properties and methods offer functionality that help you write scripts.
- Arrays and objects can be used to create complex data sets (and both an contain the other).

<br>



<br>

Chapter 5 - Document Object (pp.183-242)
<br>
**Main Points**
- The browser  represents the page using a Dom tree.
- DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes.
- You can select element nodes by their id or class attributes, by tag name, or using CSS selector syntax.
- Whenever a DOM query can return more than one node, it will always return a `NodeList`.
- From an element node, you can access and update its content using properties such as `textContent` and `innerHTML` or using `DOM` manipulation techniques.
- An element node can contain multiple text nodes and child elements that are siblings of each other.
- In older browsers, implementation of the `DOM` is inconsistent (and is a popular reason for using jQuery).
- Browsers offer tools for viewing the DOM tree.

## **Article** <br>

[Understanding the problem domain is the hardest part of programming.](https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming) <br>
The hardest part about writing code?
  - Learning a new technology
  - Naming things
  - Debugging
  - Fixing bugs
  - Making sofware maintainable

**But really the biggest problem is learning the problem domain.**

- A familiar problem.

- Why prolem domains are hard.
  1. Figure out what the major components of the picture are
  1. Sort the pieces by color or component
  1. Put together all the border pieces
  1. Put together each component of the picture from  the piles you created

- Programming is easy if you understand the problem domain.

- What can you do about it?
  1. Make the problem domain easier.
  1. Gt better at understanding th problem domain.

The hardest part is not having enough information when working with the problem domain and that will make the whole process much much harder to  complete. Having others tell you where there are tested problems and what needs work. Having all the specs is key! Working with a problem domain is like a jigsaw puzzle and you need all the important pieces to start first.

[Back to 201 Index](201-index.md)<br>
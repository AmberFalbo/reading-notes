# Read: 06 - JS Object Litrals; The Dom

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

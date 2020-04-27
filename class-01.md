# Read: 01 - Intoductory HTML and JavaScript

**HTML & CSS**
* Chapter 1 - Structure
* Chapter 8 - Extra Markup
* Chapter 17 - HTML5 Layout
* Chapter 18 - Process & Design
**JavaScript & jQuery**
* Chapter 1 - The ABC of Programming

>HTML & CSS <br>
Jon Ducket

## **Structure** *(chapter 1)*

The building of your skeleton!
* HTML code is made up of characters that live inside angled brackets - these are called HTML **elements.** 
* Elements are usually made up of two **tags:** an opening tag and a closing tag. (The closing tag has a backslash at the beginning of it.)
* Each HTML element tells the browser something about the information that sits between its opening and closing tags.
* Tags act like containers!


![dino skeleton](https://cdn8.picryl.com/photo/1895/12/31/skeleton-from-manual-of-geology-treating-of-the-principles-of-the-science-with-e167a1-1024.jpg)

## **Extra Markup** *(chapter 8)*

* Specifying different versions of HTML
* Identifying and grouping elements
* Comments, meta information and iframes

 **Doctypes** - each webpage should begin with a DOCTYPE declaration to tell a browser which version of HTML the page is using.

 ```
 <!DOCTYPE html>
 ```

**Comments in HTML** - it's a good idea to add comments to your code because, no matter how familiar you are with the page at the time of writing it, when you come back to it later the comments will make it much easier.

```
<!--  -->
```

**ID Attribute** - this is used to uniquely identify that element from other elements on the page. It's value should start with a letter or an underscore (not a number or any other character). *It is important that no two elementes on the same page have the same value for their id attributes (otherwise the value is no longer unigue).*

```
<p>
</p>
<p id="pullquote> this part bcome larger and all caps.
</p>
<p>
</p>
```

**Class Attribute** - this makes it possible to indentify several elements as being different from the other elements on the page. The class attribute on any element can share the same value.

```
<p class="important"> this is big, bold & caps
</p>
<p>
</p>
<p class="important admittance"> this is caps and in red
</p>
```



## **HTML5 Layout** *(chapter 17)*

* Introducing a new set of elements that help define the structure of your page.
  
    
![elements](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcROdIvUmb9yr9pRujQLBFONycQLT-Ykf_n_QgvJ44U14VmszhAt&usqp=CAU)


## **Process & Design** *(chapter 18)*

So you're ready to build your own website!
* Understand the audience your site may attract and what information they will expecto to find on it.
    * Every website should be designed for the target audience - not just for yourself or the site owner.
    * Invent some fictional visitors from your typical target audience. 
* What are you trying to achieve?
    * set **Key Motivations & Specific Goals**
>JavaScript & jQuary <br>
Jon Ducket

## **The ABC of Programming** *(chapter 1)*

* **A** - what is a script and how do I create one?
    * a script is a series of instructions that the computer can follow in order to achive a goal.
    * each time the scipt runs, it mmight only use a subset of all the instructions.

* **B** - how do computers fit in with the world around them?
    * computers create models of the world using data.
    * the models use objects to represent physical things.
    * objects can have: properties that tell us about the object; methods that perform tasks using the properties of that object; events which are triggered when a user interacts with the computer.

* **C** - how do I write a script for a web page?
    * it is best to keep JavaScript code in its own JavaScript file. JavaScript files are text files (like HTML pages and CSS style sheets), but they have the **.js** extention.
    * The HTML **< script >** element is used in HTML pages to tell the browser to load the JavaScript file (rather like the **< link >** element can be used to load a CSS file).

    <br>
    <br>
![cat party](https://upload.wikimedia.org/wikipedia/commons/thumb/1/15/Louis_Wain_The_bachelor_party.jpg/800px-Louis_Wain_The_bachelor_party.jpg)

[Main](https://amberfalbo.github.io/learning-journal/)

# Structure web pages with HTML

## References **Duckett: HTML & CSS**
* Chapter 18 - Process & Design
    * building a site from scratch **tahdah**
    * think about the type of page you would like to build.
* Chapter 1 - Structure
    * Review of Code 101
* Chapter 17 - HTML5 Layout
    * Note how thes element are common to the vast majority of web pages.
* Chapter 8 - Extra Markup

## first off lets start from the beginning...

## **Structure** *(chapter 1)*

The building of your skeleton!
* HTML code is made up of characters that live inside angled brackets - these are called HTML **elements.** 
* Elements are usually made up of two **tags:** an opening tag and a closing tag. (The closing tag has a backslash at the beginning of it.)
* Each HTML element tells the browser something about the information that sits between its opening and closing tags.
* Tags act like containers!


![dino skeleton](https://svgsilh.com/svg/2525420.svg)

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
  
    
![elements](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRBD6qRRURzXMupLQ9bd4SDsRvjiJebntbB2C6f67G24fqNDlXd&usqp=CAU)


## **Process & Design** *(chapter 18)*

So you're ready to build your own website!
* Understand the audience your site may attract and what information they will expecto to find on it.
    * Every website should be designed for the target audience - not just for yourself or the site owner.
    * Invent some fictional visitors from your typical target audience. 
* What are you trying to achieve?
    * set **Key Motivations & Specific Goals**

![cat party](https://www.publicdomainpictures.net/pictures/310000/velka/cats-party-at-the-campfire.jpg)

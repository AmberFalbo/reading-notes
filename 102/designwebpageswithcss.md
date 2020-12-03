[Main](https://amberfalbo.github.io/learning-journal/)

# Design web pages with CSS

### file structure and organization
Create a top level folder projects/102
Put all repositories in the 102 folder

### terminal command
mv - move command also used for renaming
cp - copy command

### CSS - Cascading Style Sheets
Pretty Stuff
CSS is a time suck

### items to look for: ref. Pg 232
All ch. 10
CSS - Cascading Style Sheets - a declarative syntax for defining the presentation of a web pages.
Element - this function in CSS defines an <image> value generated from an arbitrary HTML element. This image is live, meaning that if the THML element is changed, the CSS properties using the resulting value are automatically updated.
Selector - indicates which element the rule applies to. The same rule can apply to more than one element if you operate the element names with commas.
Properties - indicate the aspects of the element you want to chane. For example, color, font, width, height and border.
Value - specify the settings you want to use for the chosen properties. For example, if you want to specify a color property then the value is the color you want they text in these elements to be.
Css rule - (pg 236) can be included in an HTML page by placing them inside a <style> element, which usually sits inside the <head> element of the page. Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that indicate what these elements should look like). CSS rules usually appear in a separate docuent, although they may appear within an HTML page.
Declaration - indicates hot the element referred to in the selector child be styled. Declarations a are split into two parts ( a property and a value), and are separated by a colon. 

(extra on summary pg244)

Ch 11
RGB values - values for red, green, and blue are expressed as numbers between 0 and 255. ex. rgb (102, 205, 170) “this color is made up the following values: 102 red 205 green 170 blue”

Hex codes - hex values represent values for red, green, and blue, in hexademicl code.
ex. #66cdaa “ the value of th red, 102, is expressed as 66 in hexadecimal code. The 205 of the green is expressed as cd and the 170 os the blue equates to aa.

HSL - CSS3 colors (255)
	Hue - hue is the colloquial idea of color. In SSL colors, hue is often represented as a color circle where the angle represents the color, although it may also be shown as a slider with values from  0 to 360. 
	saturation - is the amount of gray in a color. Saturation is represented as a percentage 100% is full saturation and 0% is a shade of gray. 
	Lightness - is the amount of white (lightness) or black (darkness in a color. Lightness is represents das a percentage 0% lightness is black , 100% lightness is white, and 50% lightness is normal. Lightness is sometimes referred as luminosity.

HSLA - is the above but with an additional “a”
	Alpha - this is express as a number between 0 and 1.0 for example, 0.5 represents 50% transparency, and 0.75 represents 75% transparency.
   

Use information from summary on page!

Vocab for class not listed above

Curly braces (sourse online) - the curly braes and everything inside is a declaration block. The bit before the opening cult brace is a selector. Each key/value pair, as departed by a colon and ending in a semicolon, is a declartion. Also see DELCLARation

Create- 

Terminal:  Touch styles.css

Link to html-

In head of html page: <link href=“styles.css” type=“text/css” rel=“stylesheet”/> (the backslash is optional)
(a cheet is to link then import but fix styles)

-prestyling is related to the browser/broswers sometimes have similar styles but also can be ‘off’

-CSS reset- meyerweb ( you can copy and paste this reset) create a reset.css, add reset ABOVE the first style.CSS link(if not it will reset all the css work you did), this takes away all restyling so you can complete control on what your site is doing, makes you unreliant on what your browser does) - RESET will be used in 201


In style.CSS page

Look at HTML and look at what line and tag needs to be altered before going into CSS


Rule: the section is a selector, can add to multiple pages
Section {
	background-color: bisque;
	border: solid black 2 px;
}

Change learn to become a Sith lord: the tag is h1

h1{
	text-align(declaration): center;
}

Center image: give the specific image an id “pic1” within the HTML
Diference between id and class - there can only be one id, classes can be assigned to multiple tags.
In HTML 
<img id=“pic1” src=“https://live.staticflickr.com/5236/705

In CSS: using the ID to talk to image to center image

#pic1 {
	display: block;
	margin-left: auto;
	margin-right: auto;
	width: 50%;
}
Or
	margin: auto;

Above is responsive with page!

(you use chrome for dev tools, right click and inspect the cod and target the elements)
(the box model, how you can use padding, border and margin to move things around on website, USE IT TO FIND THE CONTENTS, you can apply to padding and it won’t effect margin (more in 201))


No id: will effect all images
But an ID wins over all, then class then other

Stylize the nav bar: (the reset would get rid of bullet points

ul  li {
	display: inline;
}(took away bullot points then the added li made them on the same row)

again without and ID it will effect all ul’s and li’s

create class in html:
class=“nav” and add to all ul and li you want targeted
 

			<ul class=“nav”>
ex of more id and class	<li id=“about” class=“nav” >about us</li>
				<li class=“nav” >mision statement</li>
				<li class=“nav” >home</li>
				<li class=“nav” >contact us</li>
			</ul>


to taget class

.nav {
	display: inline;
	border: (add border to the specific id) solid black 1px;
	margin: auto;
}

wildcard:effects all borders/great while developing to view the sections

*{
	border: solid black 1px
}


how to target specific nav li’s:

nav > ul > li (contains all elements on left {
	margin: 10px 20px; (top and bottom then left and right) 
	margin: 10px 20px 5px 8px; or with 4 (top right bottom left)
	
	margin: 70px (pushing from each other
	padding: 10px (starting to move)
	}
	
	in footer make the words little images with hrefs
	add a copyright symbol

add color: 

margin: 70px (pushing from each other
	padding: 10px (starting to move)
	color: blue;	
}

make ID on a li
#about {
	color: orange;
	background 
}


.= for class
#= for id

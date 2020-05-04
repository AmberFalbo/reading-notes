Career: Partner Power Hour, Report #1
Dale Sande is about to start! Join us at 12:15 to learn all about web components
Alaska Airlines
lit elements, web coponents
the wow factor of design

frame works using primative web

how primatives should be use
frameworks with strong opinions
opinions lead to standards

standards are everywhere

strong opioiions changes what happens in the standards community

frameworks talk about components and how to build them

what does it mean to build web compotents in the browser

twitter: @anotheruiguy
Previously worked for microsoft - project microsoft web foundation (now, the new fluid concept) (UI fabric connection of ui components)
senior engineer with alaska airlines
wild about web components

design		/		code

core products used for travel made by possibly just 3 people

design systems
bootstrap
material ui

Drive Design consistancey

’Sketch’ (design)		/		HTML/Sass (code)

great ui assets		/		doesnt work well together

copy/paste HTML will mutate!!!

Contracts will be broken!!

CSS nameing conventions are DOOMED to fail!!

“But, devs wil make things from my things?” 

Does not solve the CSS problem, engineers struggle with CSS!!!

CSS in JS is only masking the issue
 
I no want another monolithic UI framework - engineers don’t want another monolithic UI


’Sketch’ (design)		/		Web components
good			/		good!!

encapsulated CSS. Done. JS. Done. UX. Done.

What happens in the shadowDOM … stays in the shadowDOM

Delifver as versioned packages

IMport to your poroject and profit

with web components you have instant consistancy!!!


where can you use custom elemnet aka web components?

custom elements can be used everywhere!

what he does!!
**produce documentation with how to use web components
** react will release a version to work with web components


browser support
most all work out of the box with web components

are web compotnents ready for prime time?
-microsoft releasing github components
-apple using web components in iMusic

how do we build web components?

my-element.js (needs this naming convention)

```
import {LItElement, html} from ‘https://unpkg.com/lit-element/lit-element.js?modle';
class MyElement extens LitElement {

	render() {
		return html
TODO

```


index.html

adding static get styles


adding attribute
static get styles

components have host:
reg CSS doesn’t have host:

adding a function called mood

properties.js


my-button.js

my-element.js

span or div for button

<span> is good because it’s “pointless”


explian API
make it so the engineer just needs to add html!!
SUPER FLEXIBLE!!

what about the CSS?
	WC-/-render

accesbility DOM (object model)

this will be great to use for job use!!
AWESOME PERFORMANCE!!
Solves the CSS problem
plays well with others
Accessiility support

you can bake accessibility features into the component!!

helps from failing the audit!!


	Coaching would be the biggest drawback to getting a company to switch to web 		components
	people don’t want to switch from what they are used to
	You will need to be a cheerleader for web components to get others on board 

PERSERVERINCE IS THE DIFFERENCE BETWEEN A GREAT DEV AND A CRAPPY DEV!!

check out!!
open-wc
lit element
lit html
lying 
web components/alaska airlines

learning web components as a newB
read the lit element api
a lot in the alaska repo (component generator - strong opinion about how its cobbled together)
follow - justin faganiti (find in repo)
read about parcel in the repo (in generator)
https://alaskaairlines.github.io/ods-button/

 YOU AREN’T GOING TO LEARN IT ALL AT ONCE BUT IT ALL IS A RESOURCE!!!

BLOG WHAT YOU LEARN!! you can read it later!!






#Cascading Style Sheets
CSS is a language used to describe the appearance and formatting of your HTML.

A style sheet is a file that describes how an HTML file should look.

##How to link CSS to the HTML
To link a stylesheet to a HTML document, we place the code below in the `<head>` tag of the html document
```
<link type="text/css" rel="stylesheet" href="style.css">
```

* A `type` attribute that should always be equal to `"text/css"`
* A `rel` attribute that should always be equal to `"stylesheet"`
* A `href` attribute that should point to the web address of your CSS file (or where the css is saved) 


##Why is CSS useful 

* apply the same formatting to several HTML elements without rewriting code 
* You can apply similar appearance and formatting to several HTML pages from a single CSS file

##Syntax for CSS
**All html elements are selectors**
```
selector {
    property: value;
}
```

* A selector can be any HTML element, such as `<p>`, `<img>`, or `<table>`.
* A property is an aspect of a selector. For instance, you can change the font-family, color, and font-size of the text on your web pages
*  value is a possible setting for a property. color can be red, blue, black, or almost any color; font-family 

For Example

```
p {
    color: red;
}
```
You need to end each property-value with a semi-colon (;). That's how CSS knows you're done with one pair and ready for the next.

In CSS you can have **many properties** in **one selector** 

##Comments in CSS 
Comments in css are written as follows 

`/*I'm a comment!*/`


##Pixels and ems
Adjusting font size can be done using pixels `px` or `em`s

A pixel is a dot on your computer screen. Specifying font sizes in pixels is great when you want the user to see exactly on their screen what you designed on yours, though it assumes your screens are of similar size.

`em` is a relative measure: one `em` is equal to the default font size on whatever screen the user is using. That makes it great for smartphone screens, since it doesn't try to tell the smartphone exactly how big to make a font.

It means -

`1em` is the font size that is normally used, so `2em is twice as big and `0.5em` is half that size


#Positioning in CSS

`margin: auto;` is the CSS used to tell the browser: set equal margins on each side of this HTML element." When the margins are equal, the object is centered.

`text-align: center;` is how you center text elements.

#Multiple Selectors 

So what if you want to grab `<p>`s that are inside two `<div>`s, and not all `<p>`s?

For example

```
<div>
    <div>
        <p>I like tacos!</p>
```
We use the following to do this 

```
div div p {
    /*CSS stuff!*/
}
```

#Selecting direct children
If you want to grab direct children—that is, an element that is directly nested inside another element, with no elements in between—you can use the > symbol, like so:

```
div > p { /* Some CSS */ }
```
This only grabs `<p>`s that are nested directly inside of `<div>`s; it won't grab any paragraphs that are, say, nested inside lists that are in turn nested inside `<div>`s.

#Classes `.`

Classes are useful when you have a **bunch of elements** that should **all receive the same styling**. Rather than applying the same rules to several selectors, you can simply **apply the same class to all those HTML elements**, then **define the styling for that class in the CSS tab**.

Classes are identified in CSS with a dot `(.)`


##How to change a class using CSS
```
.square {
    height: 100px;
    width: 100px;
}
```

#IDs `#`

IDs, are used when you have exactly one element that should receive a certain kind of styling.

IDs are identified in CSS with a hash symbol `(#)`

##How to change an ID using CSS

```
#first {
    height: 50px;
}

#second {
    height: 100px;
}

#intro {
    color: #FF0000;
}
```






##Example of CSS

```
color: yellow;  
background-color:#a1a1a1;  
font-size: 12px;  
property: value;
```


**The # indicates the ID**



#How to change the first element in a class 

```
#sect1 > h2 {
color:red;
}
```

#How to change all elements in a class

```
#sect1 h2 {
color:red;
}
```
Selector type 
id 
class

padding 

#Advanced CSS
Display types
 
* block (box) -  div,h1,p is block by default
* inline - wrapped in a span tag, sits on the same line as surrounding text. text or element will be inline with content around it. cannot apply width and height to inline elements. images are inline, span, 
* inline-block - 
* none - removed element from display on the page

#The Box Model
![The Box Model] (http://scm.ulster.ac.uk/~B00662725/COM202/Images/box.gif)


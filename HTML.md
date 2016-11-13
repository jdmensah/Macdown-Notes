#HTML & CSS Information 
[Codeacademy HTML Course] (https://www.codecademy.com/learn/web)

HTML is used to give websites stucture  
We open HTML files using a browser, and the browser renders (shows us) the file


* Documents always starts with `<!DOCTYPE html>` tag (Cap Sensitive)   
This tells the browser what language it's reading (in this case, HTML).
* Always put `<html>` on the next line. This starts the HTML document.
* Always put `</html>` on the last line. This ends the HTML document.

Everything written in a HTML document goes between the `<html>` tags 

--

#The Head Tag `<head>`

The head contains information about your HTML file, like its title. The title is what we see in the browser's title bar or page tab.

--

#The Body Tag `<body>`

The body is where you put your content, such as text, images, and links. The content in the body is what will be visible on the actual page.

* The body goes inside the `<html>` tags, right after the `<head>` tags.

For example 

```html
<html>
  <head>
    <title>My Webpage</title>
  </head>
  
  <body>
  </body>
  
</html>
```
--
#Headings `<h#>`

Headings are used to chagne the size of text i.e the heading of a section of writing. There are 6 headers these are: 

```html
<h1>test</h1>
<h2>test</h2>
<h3>test</h3>
<h4>test</h4>
<h5>test</h5>
<h6>test</h6>
```
### Code In Use Below
<h1>test</h1>
<h2>test</h2>
<h3>test</h3>
<h4>test</h4>
<h5>test</h5>
<h6>test</h6>
--

#Hyperlinks `<a href>`
Hyperlinks are used to navigate the user to one sections of the website to another. This can be on the host website or to a completely different website. 

* First, there's an opening `<a>` tag and that tag has an *attribute* called ***href***. The href value tells your link where you want it to go, eg. www.google.com
* Then you have a description of your link between your opening `<a>` and your closing `</a>` tags. This is what you will be able to click on.

For Example

```html
<!DOCTYPE html>
<html>
	<head>
		<title></title>
	</head>
	<body>
	    <a href="www.google.com"> Google.com </a> 
	</body>
</html>
```
### Code In Use Below  
<a href="www.google.com"> This is a link to Google </a>

-- 

#Images `<img src>`
We use an image tag, like so: `<img>`. This tag is a bit different from the others. Instead of putting the content between the tags, you tell the tag where to get the picture using src. It's also different because there is no ending tag. It has `/` in the tag to close it: `<img src="url" />`. 

For example

```html
<!DOCTYPE html>
<html>
	<head>
		<title></title>
	</head>
	<body>
		<img src="https://s3.amazonaws.com/codecademy-blog/assets/f3a16fb6.jpg" />
	</body>
</html>
```
### Code In Use Below
<img src="https://s3.amazonaws.com/codecademy-blog/assets/f3a16fb6.jpg" />
`<img src="https://s3.amazonaws.com/codecademy-blog/assets/f3a16fb6.jpg" />`
Note how the the ending tag is a simple `/>` and not a closing tag like others.

--
#Making Pictures Into Links `<a href=...> <img src> </> </a>`
* Open up the `<a>` tag and point the href to the website of your choosing.
* Instead of using text inside the `<a>` tag, we use the `<img>` tag.
* Remember to close using `</a>`

For Example 

```html
<!DOCTYPE html>
<html>
	<head>
		<title></title>
	</head>
	<body>
		<a href="https://www.google.co.uk"> <img src="https://s3.amazonaws.com/codecademy-blog/assets/f3a16fb6.jpg" /></a>
	</body>
</html>
```
Note the where you normally place text in the link tag is replaced with the `<img>`syntax. Compare below

**Normal Hyperlink Tag Syntax**  
<a href="www.google.co.uk"> The is a link to google </a> 
`<a href="www.google.co.uk"> The is a link to google </a>`

**Image Hyperlink Tag Syntax**  
<a href="https://www.google.co.uk"><img src="https://s3.amazonaws.com/codecademy-blog/assets/f3a16fb6.jpg"/></a>
`<a href="https://www.google.co.uk"><img src="https://s3.amazonaws.com/codecademy-blog/assets/f3a16fb6.jpg"/></a>`

--

#Ordered Lists `<ol>` & `<li>`

An ordered list is simply a list that is numbered

* we begin the ordered list with the opening tag `<ol>` 
* we wrap (i.e. surround) each individual item with `<li>` and `</li>` tags.
* Because each listed item is only on one line, we put the entire element on one line.
*  we finish the ordered list with the closing tag `</ol>`

For Example  
		<ol> 
		    <li>CD</li>
		    <li>Bag</li>
		    <li>Headphones</li>
		    <li>Laptop</li>
		</ol>

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Lists</title>
	</head>
	<body>
	
	    <h1> New Ordered List</h1>
		<ol> 
		    <li>CD</li>
		    <li>Bag</li>
		    <li>Headphones</li>
		    <li>Laptop</li>
		</ol>
		
	</body>
</html>
```
##Unordered Lists
Unordered lists behave in the same fashion. Simply change the `<ol>` (ordered list) tag with `<ul>` (unordered list) tag.

For example 
		<ul> 
		    <li>CD</li>
		    <li>Bag</li>
		    <li>Headphones</li>
		    <li>Laptop</li>
		</ul>

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Lists</title>
	</head>
	<body>
	
	    <h1> New Ordered List</h1>
		<ul> 
		    <li>CD</li>
		    <li>Bag</li>
		    <li>Headphones</li>
		    <li>Laptop</li>
		</ul>
		
	</body>
</html>
```
##List Inside a List
f you have an ordered list, but each item in the ordered list also has an unordered list nested in it? Nested simply means 'inside' the list. 

For Example
		<ul>
		    <li>Favourite Boys' Names</li>
		    <ol>
		    <li>Jack</li>
		    <li>James</li>
		    <li>Jason</li>
		    </ol>
		    <li>Favourite Girls' Names </li>
		    <ol>
		    <li>Helen</li>
		    <li>Steph</li>
		    <li>Beth</li>
		    </ol>
		</ul>

```html
		<ul>
		    	<li>Favourite Boys' Names</li>
		    <ol>
		    	<li>Jack</li>
		    	<li>James</li>
		    	<li>Jason</li>
		    </ol>
		    	<li>Favourite Girls' Names</li>
		    <ol>
		    	<li>Helen</li>
		    	<li>Steph</li>
		    	<li>Beth</li>
		    </ol>
		</ul>
```	
--
#The Style Attribute `style=...:`

##Font Size `< style="font-size: 12px">`

We can give tags more instructions by including attributes in the opening tag. An attribute is simply a characteristic or some description for the content in the element.

To chagne the size of the text, we use the style attribute. We make it equal to font-size, followed by a colon, the size you want, and end it with px (short for "pixels"). 

```html
<p style="font-size: 12px">
```

For Example

```html
<p style="font-size:10px"> Some text for you to make tiny! </p>
<p style="font-size:20px"> Some text for you to make normal size!</p>
<p style="font-size:40px"> Some text for you to make super big!</p>
```
<p style="font-size:10px"> Some text for you to make tiny! </p>
<p style="font-size:20px"> Some text for you to make normal size!</p>
<p style="font-size:40px"> Some text for you to make super big!</p>

##Font Color `< style="color:red">`
To change the color of text, simply add the style attribute in the opening tag, then make the style equal to "color:blue" (or whatever color you like). For example:

`<h2 style="color:red">`

If you want to change the color and the size of the text add a semi-colon between each bit. For example:

`<h2 style="color: green; font-size:12px">`

For Example

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Changing the colors!</title>
	</head>
	<body>
		<h1 style="color: green;font-size: 16px">Big Heading</h1>
			<p style="color: violet">A giant bear and a little duck were friends.</p>
			<p style="color: red;font-size:10px">But the bear got hungry and ate the duck.</p>
	</body>
</html>
```
<p style="color:red"> This is red text </p>

##Font-family `<style="font-family: Arial">`

Similar to other tags to change the font of text in html you use `font-family`

For Example 

<p style="font-family: Verdana">Title</p>

```
<p style="font-family: Verdana">Title</p>
```
##Background Color `<style="background-color:red">`

To change the background color of text we use `background-color`

For example  
<p style="background-color:red"> Jason</p>
```
<p style="background-color:red"> Jason</p>
```

##Alinging Text 
To align text we again use the style attribute. And then we use "text-align:left" (or right, or center) to determine the location of the text.

`<h1 style="text-align:center">`
`<h1 style="text-align:right">`
`<h1 style="text-align:left">`

For Example 
<h3 style="text-align:center"> List</h3>
<p style="text-align:center"> Jason </p>
<p style="text-align:right"> John </p>
<p style="text-align:left"> Dzela </p>

--
#Making a word BOLD `<strong>`
To make a word bold we use the `<strong>`tag 

For Example 
<p><strong>Jason</strong></p>
`<p><strong>Jason</strong></p>`

Remember to close the tags 

--
#How to emphasize a word `<em>`
we often want to italicize words and to do that we use `<em>`

For Example 
<p style="font-family:Verdana"> Jason Dzela-<em>Mensah</em></p>
`<p style="font-family:Verdana"> Jason Dzela-<em>Mensah</em></p>

--
#Tables `<table>`
When you want to present information neatly in a table with rows and columns we use the `<table>` tag 

To add rows to the table we use the `<tr>`tag (table row) 

To add table cells where we can input data we us use the `<td>`tag (table data).

<table border="1px">
	<tr>
	<td>One</td>
	</tr>
	<tr>
	<td>Two</td>
	</tr>
	<tr>
	<td>Three</td>
	</tr>
</table>

```
<html>
    <head>
        <title>Table Time</title>
    </head>
    
    <body>
        
        <table border="1px">
            <tr>
                <td>One</td>
            </tr>
            
            <tr>
                <td>Two</td>
            </tr>
            
            <tr>
                <td>Three</td>
            </tr>
        </table>
        
    </body>

</html>
```
##Head of the table
To make our table look a little more like a table, we use the <thead> and <tbody> tags. These go within the <table> tag and stand for table head and table body, respectively.

The `<head>` HTML tag contains information about a web page (e.g. its title) and the `<body>` tag contains the contents of the web page. In the same way, the `<thead>` tag can be thought of as containing information about a table and the `<tbody>` tag containing the actual tabular data.


#finish off the table section 

#Div `<div>`

`<div>`is short for division allow you to divide your page into containers 

For Example 

```
<div>
<p>This is an example of a div</p>
</>
```

#Span `<span>`

`<span>` allows you to control styling for smaller parts of your page 

```
<p>This text is black, except for the word <span style="color:red">red!</span></p>
```

#Parents, children, and siblings
If you think of the `<html>` tag as the trunk of the tree, you can think of its immediate branches—`<head>` and `<body>`—as its **children**. Both tags are **children** of `<html>`, and `<html>` is their **parent** element. Because they are both **immediate children** of `<html>` (that is, they are both only one element away), they are **siblings**.

For Example

```
<!DOCTYPE html>
<html> <!--The trunk of the tree!-->
	<head> <!--Child of html, parent of title,
		   sibling of body-->
		<title></title> <!--Immediate child of head,
						child of head AND html-->
	</head>
	<body> <!--Child of html, parent of p,
		   sibling of head-->
		<p></p> <!--Immediate child of body,
				child of body AND html-->
	</body>
</html>
```

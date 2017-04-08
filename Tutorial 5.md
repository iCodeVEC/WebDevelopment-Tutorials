# CSS
CSS refers to <b>C</b>ascading <b>S</b>tyle <b>S</b>heets.<br>
CSS is a language that describes the style of an HTML document.<br>
CSS describes how HTML elements should be displayed.
## Example Program
```
<!DOCTYPE html>
<html>
<head>
<style>
body {
    background-color: lightblue;
}

h1 {
    color: white;
    text-align: center;
}

p {
    font-family: verdana;
    font-size: 20px;
}
</style>
</head>
<body>

<h1>My First CSS Example</h1>
<p>This is a paragraph.</p>

</body>
</html>
```
# CSS Syntax
A CSS rule-set consists of a selector and a declaration block.
<table>
<tr>
<th> Selector </th>
<th> Declaration </th>
</tr>
<tr>
<td>h1</td>
<td>{color:blue; font-size:12px;}</td>
</tr>
</table>
The selector points to the HTML element you want to style.<br>
The declaration block contains one or more declarations separated by semicolons.<br>
Each declaration includes a CSS property name and a value, separated by a colon.<br>
A CSS declaration always ends with a semicolon, and declaration blocks are surrounded by curly braces.<br>
## Example Program
```
<!DOCTYPE html>
<html>
<head>
<style>
p {
    color: red;
    text-align: center;
} 
</style>
</head>
<body>
<p>Hello World!</p>
<p>These paragraphs are styled with CSS.</p>
</body>
</html>
```
# CSS Selectors
CSS selectors are used to "find" (or select) HTML elements based on their element name, id, class, attribute, and more.
## Types of Selectors 
1.Universal Selector<br>
2.Element Type Selector<br>
3.ID Selector<br>
4.Class Selector<br>
5.Descendant Selector<br>
## Universal Selector
The universal selector works like a wild card character, selecting all elements on a page.<br> 
Every HTML page is built on content placed within HTML tags.<br> 
Each set of tags represents an element on the page.
## Snippet 
```
* {
   color: green;
   font-size: 20px;
   line-height: 25px;
}
```
## Element Type Selector
Also referred to simply as a “type selector,” this selector must match one or more HTML elements of the same name.
## Snippet
```
ul {
   list-style: none;
   border: solid 1px #ccc;
}
<ul>
  <li>Fish</li>
  <li>Apples</li>
  <li>Cheese</li>
</ul>
<div class="example">
  <p>Example paragraph text.</p>
</div>
<ul>
  <li>Water</li>
  <li>Juice</li>
  <li>Maple Syrup</li>
</ul>
```
## ID Selector
An ID selector is declared using a hash, or pound symbol `(#)` preceding a string of characters.<br> 
The string of characters is defined by the developer.<br> 
This selector matches any HTML element that has an ID attribute with the same value as that of the selector, but minus the hash symbol.
## Snippet 
```
#container {
   width: 960px;
   margin: 0 auto;
}
<div id="container"></div>
```
## Class Selector
The class selector is the most useful selector of all the CSS selectors.<br> 
It is declared with a dot preceding a string of one or more characters.<br> 
Just as is the case with an ID selector, this string of characters is defined by the developer.<br> 
The class selector also matches all elements on the page that have their class attribute set to the same value as the class, minus the dot.
## Snippet
```
.box {
   padding: 20px;
   margin: 10px;
   width: 240px;
}
<div class="box"></div>
```
## Descendant Selector
The descendant selector or, more accurately, the descendant combinator lets you combine two or more selectors 
so you can be more specific in your selection method. 
## Snippet
```
#container .box {
   float: left;
   padding-bottom: 15px;
}
```
This declaration block will apply to all elements that have a class of box that are inside an element with an ID of `container`.<br> 
It is worth noting that the `.box` element doesn’t have to be an immediate child there could be another element wrapping `.box`, 
and the styles would still apply.
```
<div id="container">
  <div class="box"></div>
      <div class="box-2"></div>
</div>
<div class="box"></div>
```
If we apply the CSS in the previous example to this section of HTML, the only element that will be affected by those styles is the first `<div>` element that has a class of `box`.<br>
The `<div>` element that has a class of `box-2` won’t be affected by the styles.<br>
Similarly, the second `<div>` element with a class of box won’t be affected because it is not inside an element with an ID of `container`.<br>
## Grouping Selectors
It will be better to group the selectors, to minimize the code.<br>
To group selectors, separate each selector with a comma.
## Example Program
```
<!DOCTYPE html>
<html>
<head>
<style>
h1, h2, p {
    text-align: center;
    color: red;
}
</style>
</head>
<body>
<h1>Hello World!</h1>
<h2>Smaller heading!</h2>
<p>This is a paragraph.</p>
</body>
</html>
```
# CSS StyleSheets
When a browser reads a style sheet, it will format the HTML document according to the information in the style sheet.
## Three Ways to Insert CSS
There are three ways of inserting a style sheet:<br>
1.External Stylesheet <br>
2.Internal Stylesheet <br>
3.Inline Stylesheet <br>
## External Stylesheet
With an external style sheet, you can change the look of an entire website by changing just one file.<br>
Each page must include a reference to the external style sheet file inside the `<link>` element.<br> 
The `<link>` element goes inside the `<head>` section.
An external style sheet can be written in any text editor. <br>
The file should not contain any html tags. <br>
The style sheet file must be saved with a .css extension.
## Example Program
```
<html>
<head>
<link rel="stylesheet" type="text/css" href="style1.css" title="style1" />
<link rel="alternate stylesheet" type="text/css" href="style2.css" title="style2" />
</head>
<body>
<h1>This is a heading </h1>
<p>This is a paragraph</p>
</body>
</html>
```
## Style1.css
```
body {
    background-color: lightblue;
}
h1 {
    color: green;
    margin-left: 20px;
}
p{
color:blue;
}
```
## Style2.css
```
body {
    background-color: lightblue;
}
h1 {
    color: red;
    margin-left: 20px;
}
p{
color:grey;
}
```
## Internal Stylesheet
An internal style sheet may be used if one single page has a unique style.<br>
Internal styles are defined within the `<style>` element.
## Example Program
```
<!DOCTYPE html>
<html>
<style>
body {
    background-color: linen;
}
h1 {
    color: maroon;
    margin-left: 40px;
} 
</style>
<body>
<h1>This is a heading</h1>
<p>This is a paragraph.</p>
</body>
</html>
```
<b>NOTE:</b>Do not add a space between the property value and the unit `(such as margin-left: 40 px;)`.<br>
The correct way is: `margin-left: 40px;`.
## Inline Stylesheet
An inline style may be used to apply a unique style for a single element.<br>
To use inline styles, add the style attribute to the relevant element.<br>
The style attribute can contain any CSS property.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<h1 style="color:blue;margin-left:30px;">This is a heading</h1>
<p>This is a paragraph.</p>
</body>
</html>
```
# CSS Navigation Bars
Having easy-to-use navigation is important for any web site.<br>
With CSS you can transform boring HTML menus into good-looking navigation bars.<br>
<b>Navigation Bar = List of Links</b><br>
A navigation bar is basically a list of links, so using the `<ul>` and `<li>` elements makes perfect sense.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>
<p>Note: We use href="#" for test links. In a real web site this would be URLs.</p>
</body>
</html>
```
## Example Program
```
<!DOCTYPE html>
<html>
<head>
<style>
ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
    background-color: #333;
}

li {
    float: left;
}

li a {
    display: block;
    color: white;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
}

li a:hover:not(.active) {
    background-color: #111;
}

.active {
    background-color: #4CAF50;
}
</style>
</head>
<body>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>
```
<b>NOTE:</b> For More Examples on Navigation Bars please refer to the following link:<br>
https://www.w3schools.com/css/css_navbar.asp
# CSS Dropdowns
Create a hoverable dropdown with CSS.
## Example Program
```
<!DOCTYPE html>
<html>
<head>
<style>
.dropbtn {
    background-color: #4CAF50;
    color: white;
    padding: 16px;
    font-size: 16px;
    border: none;
    cursor: pointer;
}

.dropdown {
    position: relative;
    display: inline-block;
}

.dropdown-content {
    display: none;
    position: absolute;
    background-color: #f9f9f9;
    min-width: 160px;
    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
    z-index: 1;
}

.dropdown-content a {
    color: black;
    padding: 12px 16px;
    text-decoration: none;
    display: block;
}

.dropdown-content a:hover {background-color: #f1f1f1}

.dropdown:hover .dropdown-content {
    display: block;
}

.dropdown:hover .dropbtn {
    background-color: #3e8e41;
}
</style>
</head>
<body>

<h2>Dropdown Menu</h2>
<p>Move the mouse over the button to open the dropdown menu.</p>

<div class="dropdown">
  <button class="dropbtn">Dropdown</button>
  <div class="dropdown-content">
    <a href="#">Link 1</a>
    <a href="#">Link 2</a>
    <a href="#">Link 3</a>
  </div>
</div>



</body>
</html>
```
## Dropdown Image
To add an image and other content inside the dropdown box.
## Example Program
```
!DOCTYPE html>
<html>
<head>
<style>
.dropdown {
    position: relative;
    display: inline-block;
}

.dropdown-content {
    display: none;
    position: absolute;
    background-color: #f9f9f9;
    min-width: 160px;
    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
    z-index: 1;
}

.dropdown:hover .dropdown-content {
    display: block;
}

.desc {
    padding: 15px;
    text-align: center;
}
</style>
</head>
<body>

<h2>Dropdown Image</h2>
<p>Move the mouse over the image below to open the dropdown content.</p>

<div class="dropdown">
  <img src="img_fjords.jpg" alt="Trolltunga Norway" width="100" height="50">
  <div class="dropdown-content">
    <img src="img_fjords.jpg" alt="Trolltunga Norway" width="300" height="200">
    <div class="desc">Beautiful Trolltunga, Norway</div>
  </div>
</div>

</body>
</html>
```















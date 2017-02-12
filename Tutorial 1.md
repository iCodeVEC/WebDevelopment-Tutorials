# Learning HTML(Hyper Text Markup Language)
At first let us start with a simple HTML program
## Example Program
```
<!DOCTYPE html>
<html>
<head>
<title>INTRO To Html</title>
</head>
<body>
<h1>This is a Heading</h1>
<p>This is a paragraph.</p>
</body>
</html>
```
#Creating Tables
Tables are used to hold values which are representated in a tabular form.<br>
An HTML table is defined with the `<table>` tag.<br>
Each table row is defined with the`<tr>`tag.<br> A table header is defined with the`<th>`tag.<br> By default,table headings are bold
and centered.<br>A table data/cell is defined with the `<td>` tag.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<table border=1 cellspacing=2 cellpadding=10 bgcolor="grey">
  <tr>
    <th>S.no</th>
    <th>Name</th> 
    <th>Age</th>
  </tr>
  <tr>
    <td>1</td>
    <td>Smith</td>
    <td>50</td>
  </tr>
  <tr>
    <td>2</td>
    <td>Jackson</td>
    <td>94</td>
  </tr>
  <tr>
    <td>3</td>
    <td>Doe</td>
    <td>80</td>
  </tr>
</table>
</body>
</html>
```
# Creating Lists
There are 3 types of lists in html:<br>
1)Ordered lists<br> 
2)Unordered lists<br>
3)Description lists<br>
## Ordered List
An ordered list starts with the `<ol>` tag.<br> Each list item starts with the `<li>` tag.<br>
The list items will be marked with numbers by default
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<h2>An ordered HTML list</h2>
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>  
</body>
</html>
```
## Unordered List
An unordered list starts with the `<ul>` tag.<br> Each list item starts with the `<li>` tag.<br>
The list items will be marked with bullets (small black circles) by default.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<h2>An unordered HTML list</h2>
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>  
</body>
</html>
```
## Description List
A description list is a list of terms, with a description of each term.<br>
The `<dl>` tag defines the description list, the `<dt>` tag defines the term (name), and the `<dd>` tag describes each term.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<h2>A Description List</h2>
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>
</body>
</html>
```
# Displaying Images 
In HTML, images are defined with the `<img>` tag.<br>The `<img>` tag is empty, it contains attributes only, and does not have a closing tag.<br>
The src attribute specifies the URL (web address) of the image.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<h2>Spectacular Mountain</h2>
<img src="1.jpg"width=304 height=200>
</body>
</html>
```
# Links In html
Links are found in nearly all web pages. Links allow users to click their way from page to page.<br>
HTML links are hyperlinks.<br>
You can click on a link and jump to another document.<br>
When you move the mouse over a link, the mouse arrow will turn into a little hand.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p><a href="1.html">Click here</a></p>
</body>
</html>
```
# Styling In Html
Setting the style of an HTML element, can be done with the style attribute.<br>
The HTML style attribute has the following syntax:<br>
`<tagname style="property:value;">`<br>
The property is a CSS property.<br> The value is a CSS value.
## Example Program 
```
<!DOCTYPE html>
<html>
<body style="background-color:powderblue;">
<p>Normal text</p>
<p style="color:red;">Hello World</p>
<p style="color:blue;">Hello World</p>
<p style="font-size:36px;">Big One</p>
<p style="font-family:courier;">This is a paragraph.</p>
<p style="text-align:center;">Centered paragraph.</p>
</body>
</html>
```
# Entities in html
Some characters are reserved in HTML.<br>
If you use the less than (<) or greater than (>) signs in your text, the browser might mix them with tags.<br>
Character entities are used to display reserved characters in HTML.<br>
A character entity looks like this:<br>
**&entity_name; (OR) &#entity_number;**

 


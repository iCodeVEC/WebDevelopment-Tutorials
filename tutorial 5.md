# CSS-BOX MODEL
##CSS box model-basic concepts and properties
## Example Program
```
<html>
<head>
<style>
div.ex
{
width:220px;
padding:10px;
border:5px solid gray;
margin:0px;
}
</style>
</head>
<body>
<div class="ex">The picture above is 250px wide.
The total width of this element is also 250px.</div>
</body>
</html>
```
#Box model shorthand properties
<b>Property<br>
1.padding-{top,right,bottom,left}<br>
2.border-{top,right,bottom,left}-width<br>
3.border-{top,right,bottom,left}-color<br>
4.border-{top,right,bottom,left}-style<br>
5. border-{top,right,bottom,left}<br>
6.margin- {top,right,bottom,left}<br>
</b>
<table border=1 cellspacing=2 cellpadding=2>
<tr>
<th>Number of Values</th>
<th>Meaning</th>
</tr>
<tr>
<td>One</td>
<td>Assign this value to all four asscoiated properties{top,right,bottom,left}</td>
</tr>
<tr>
<td>Two</td>
<td>Assign first value to associated top and bottom properties , second value to associated right and left position</td>
</tr>
<tr>
<td>Three</td>
<td>Assign first value to associated top property, second value to right and left , and third value to bottom</td>
</tr>
<tr>
<td>Four</td>
<td>Assign first value to associated top property,second to right,third to bottom and fourth to left</td>
</tr>
</table>
##Box model shorthand properties-example
```
Padding:30px is equivalent to four declaration
Padding-top:30px;
Padding-right:30px;
Padding-bottom:30px;
Padding-left:30px;
Margin:15px 45px 30px is equivalent to
Margin-top:15px
Margin-right:45px
Margin-left:45px
Margin-bottom:30px
```
#Box Model-Background Colors and Images
```
body
{
  background-image:url('paper.gif');
  background-color:#cccccc;
} 
```
The <b>border-image-repeat</b> property specifies whether the image-border should be repeated, rounded or stretched.<br>
<b>`border-image-repeat: stretch|repeat|round;`</b><br>
<b>stretch:</b><br> 
The image is stretched to fill the area <br> 
<b>repeat:</b><br> 
The image is tiled (repeated) to fill the area <br> 
<b>round:</b><br> 
The image is tiled (repeated) to fill the area.If it does not fill the area with a whole number of tiles, 
the image is rescaled so it fits.
#CSS Positioning
##Positioning
The CSS positioning properties allow you to position an element. It can also place an element behind another, 
and specify what should happen when an element's content is too big.
Elements can be positioned using the top, bottom, left, and right properties. However, these properties will not work unless the position property is set first. 
They also work differently depending on the positioning method.
There are four different positioning methods.
##Static Positioning
HTML elements are positioned static by default. A static positioned element is always positioned according to the normal flow of the page.
Static positioned elements are not affected by the top, bottom, left, and right properties.
##Float Positioning
With CSS float, an element can be pushed to the left or right, allowing other elements to wrap around it.
Float is very often used for images, but it is also useful when working with layouts.
##Fixed positioning
This type of positioning is fairly rare but certainly has its uses. A fixed position element is positioned relative to the viewport, or the browser window itself.
##Relative Positioning
A relative positioned element is positioned relative to its normal position. 
The content of relatively positioned elements can be moved and overlap other elements, but the reserved space for the element is still preserved in the normal flow.
##Absolute Positioning
Absolute positioning offers total control over the placement of boxes on the canvas.
##Example Program
```
<html>
<head>
<style>
h2.pos_left
{
position:relative;
left:-20px;
}
h2.pos_right
{
position:relative;
left:20px;
}
</style>
</head>
<body>
<h2>This is a heading with no position</h2>
<h2 class="pos_left">This heading is moved left according to its normal position</h2>
<h2 class="pos_right">This heading is moved right according to its normal position</h2>
<p>Relative positioning moves an element RELATIVE to its original position.</p>
<p>The style "left:-20px" subtracts 20 pixels from the element's original left position.</p>
<p>The style "left:20px" adds 20 pixels to the element's original left position.</p>
</body>
</html>
```
##Example Program
```
<html>
<head>
<style>
img 
{
float:right;
}
</style>
</head>
<body>
<p>In the paragraph below, we have added an image with style <b>float:right</b>. The result is that the image will float to the right in the paragraph.</p>
<p>
<img src="Water lilies.jpg" width="95" height="84" />
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
</p>
</body>
</html>
```
##Positioning Related Properties
The z-index property specifies the stack order of an element.<br>
An element with greater stack order is always in front of an element with a lower stack order.<br>
<b>NOTE:</b> z-index only works on positioned elements (position:absolute, position:relative, or position:fixed).
##Example Program
```
<!DOCTYPE html>
<html>
<head>
<style>
img {
    position: absolute;
    left: 0px;
    top: 0px;
    z-index: 1;
}
</style>
</head>
<body>
<h1>This is a heading</h1>
<img src="w3css.gif" width="100" height="140">
<p>Because the image has a z-index of -1, it will be placed behind the text.</p>
</body>
</html>
```







  
 









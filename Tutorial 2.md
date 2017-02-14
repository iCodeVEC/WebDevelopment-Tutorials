# Canvas in Html
The HTML `<canvas>` element is used to draw graphics on a web page.<br>
The HTML `<canvas>` element is used to draw graphics, on the fly, with the help of Javascript.<br>
The `<canvas>` element is only a <b>container</b> for graphics.<br> You must use JavaScript to actually draw the graphics.<br>
Canvas has several methods for drawing paths, boxes, circles, text, and adding images.<br>
The <b>syntax</b> of `<canvas>` tag looks like:<br>
`<canvas id="mycanvas" width="200" height="100"></canvas>`<br> 
<b>Note:</b> Always specify an id attribute (to be referred to in a script), and a width and height attribute to define the size of the canvas.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<canvas id="myCanvas" width="200" height="100" style="border:1px solid #000000;">
Your browser does not support the HTML5 canvas tag.
</canvas>
</body>
</html>
```
Now let us draw a rectangle using `<canvas>` and Javascript
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<canvas id="myCanvas" width="300" height="150" style="border:1px solid powderblue;">
Your browser does not support the HTML5 canvas tag.</canvas>
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.fillStyle = "#d3d3d3";
ctx.fillRect(20, 20, 150, 100);
</script>
</body>
</html>
```
# Creating iFrames
An iframe is used to display a web page within a web page.<br>
An HTML iframe is defined with the `<iframe>` tag<br>
<b>Syntax</b>:<br>
`<iframe src="URL"></iframe>`<br>
The src attribute specifies the URL (web address) of the inline frame page.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<iframe height="300px" width="100%" src="demo_iframe.htm" name="iframe_a" style="border:2px solid green">
</iframe>
<p><a href="http://www.velammal.com" target="iframe_a">W3Schools.com</a></p>
<p>When the target of a link matches the name of an iframe, the link will open in the iframe.</p>
</body>
</html>
```
# Formatting in html
HTML also defines special elements for defining text with a special meaning.<br>
Formatting elements were designed to display special types of text:<br>
`<b>` - Bold text<br>
`<strong>` - Important text<br>
`<i>` - Italic text<br>
`<em>` - Emphasized text<br>
`<mark>` - Marked text<br>
`<small>` - Small text<br>
`<del>` - Deleted text<br>
`<ins>` - Inserted text<br>
`<sub>` - Subscript text<br>
`<sup>` - Superscript text<br>
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p><b>This text is bold</b></p>
<p><i>This text is italic</i></p>
<p><em>This text is emphasized</em></p>
<p><strong>This text is strong</strong></p>
<p><mark>This text is marked</mark></p>
<p>This text is <del>deleted</del></p>
<p>This text is <ins>inserted</ins></p>
<p><small>This text is small</small></p>
<p>This is<sub> subscript</sub> and <sup>superscript</sup></p>
</body>
</html>
```

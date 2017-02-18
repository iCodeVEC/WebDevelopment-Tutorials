# HTML Javascript
The <b>`<script>`</b> tag is used to define a client-side script (JavaScript).<br>
The <b>`<script>`</b> element either contains scripting statements, or it points to an external script file through the src attribute.<br>
Common uses for JavaScript are image manipulation, form validation, and dynamic changes of content.<br>
To select an HTML element, JavaScript very often use the document.getElementById() method.
## Example Program
```
<!DOCTYPE html>
<html>
<body>	
<p id="demo"></p>
<script>
document.getElementById("demo").innerHTML = "Hello JavaScript!";
</script> 
</body>
</html>
```
This JavaScript example writes "Hello JavaScript!" into an HTML element with id="demo".
## Example Program
// <b>Date and time display program</b>
```
<!DOCTYPE html>
<html>
<body>
<h1>My First JavaScript</h1>
<button type="button"onclick="document.getElementById('demo').innerHTML = Date()">
Click me to display Date and Time.</button>
<p id="demo"></p>
</body>
</html>
```
## Example Program
// <b>Javascript change html content</b>
```
<!DOCTYPE html>
<html>
<body>
<h1>My First JavaScript</h1>
<p>JavaScript can change the content of an HTML element:</p>
<button type="button" onclick="myFunction()">Click Me!</button>
<p id="demo">This is a demonstration.</p>
<script>
function myFunction() { 
    document.getElementById("demo").innerHTML = "Hello JavaScript!";
}
</script>
</body>
</html>
```
## Example Program
// <b>Changing Html attributes</b>
```
<!DOCTYPE html>
<html>
<body>
<h1>My First JavaScript</h1>
<p id="demo">JavaScript can change the style of an HTML element.</p>
<script>
function myFunction() {
    document.getElementById("demo").style.fontSize = "25px"; 
    document.getElementById("demo").style.color = "red";     
}
</script>
<button type="button" onclick="myFunction()">Click Me!</button>
</body>
</html>
```
## `<noscript>` Tag:
The <noscript> tag is used to provide an alternate content for users that have disabled scripts in their browser 
or have a browser that doesn't support client-side scripts.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p id="demo"></p>
<script>
document.getElementById("demo").innerHTML = "Hello JavaScript!";
</script>
<noscript>Sorry, your browser does not support JavaScript!</noscript>
<p>A browser without support for JavaScript will show the text written inside the noscript element.</p>
 </body>
</html>
```
# HTML Responsiveness
Responsive Web Design makes your web page look good on all devices (desktops, tablets, and phones).<br>
Responsive Web Design is about using CSS and HTML to resize, hide, shrink, enlarge, or move the content to make it look 
good on any screen.
## Example Program
```
<!DOCTYPE html>
<html>
<head>
<style>
.city {
   float: left;
   margin: 10px;
   padding: 10px;
   max-width: 300px;
   height: 300px;
   border: 1px solid black;
}   
</style>
</head>
<body>
<h1>Responsive Web Design Demo</h1>
<h2>Resize this responsive page!</h2>
<div class="city">
  <h2>London</h2>
  <p “”>London is the capital of England.</p>
<p>It is the most populous city in the United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
</div>
<div class="city">
<h2>Paris</h2>
  <p>Paris is the capital of France.</p> 
  <p>The Paris area is one of the largest population centers in Europe, with more than 12 million inhabitants.</p>
</div>
<div class="city">
  <h2>Tokyo</h2>
  <p>Tokyo is the capital of Japan.</p>
  <p>It is the center of the Greater Tokyo Area, and the most populous metropolitan area in the world.</p>
</div>
<div class="city">
  <h2>New York</h2>
  <p>The City of New York is the most populous city in the United States.</p>
  <p>New York is an important center for international diplomacy and has been described as the cultural and financial capital of the world.</p>
</div>
</body>
</html>
```
## Example Program
//<b> Using Stylesheets</b>
```
<!DOCTYPE html>
<html>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="/lib/w3.css">
<body>
<div class="w3-container w3-orange">
  <h1>W3.CSS Demo</h1>      
  <p>Resize this responsive page!</p>      
</div>
<div class="w3-row-padding">
<div class="w3-third">
  <h2>London</h2>
  <p>London is the capital of England.</p>
  <p>It is the most populous city in the United Kingdom,
  with a metropolitan area of over 13 million inhabitants.</p>
</div>
<div class="w3-third">
  <h2>Paris</h2>
  <p>Paris is the capital of France.</p> 
  <p>The Paris area is one of the largest population centers in Europe,
  with more than 12 million inhabitants.</p>
</div>
<div class="w3-third">
  <h2>Tokyo</h2>
  <p>Tokyo is the capital of Japan.</p>
  <p>It is the center of the Greater Tokyo Area,
  and the most populous metropolitan area in the world.</p>
</div>
</div>
</body>
</html>
```
# HTML Canvas Using Javascript
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<canvas id="myCanvas" width="200" height="100"
style="border:1px solid #c3c3c3;">
Your browser does not support the canvas element.
</canvas>
<script>
var canvas = document.getElementById("myCanvas");
var ctx = canvas.getContext("2d");
ctx.fillStyle = "#FF0000";
ctx.fillRect(0,0,150,75);
</script>
</body>
</html>
```
## Example Program
//<b>Drawing Line</b>
```
<!DOCTYPE html>
<html>
<body>
<canvas id="myCanvas" width="200" height="100"
style="border:1px solid #d3d3d3;">
Your browser does not support the canvas element.
</canvas>
<script>
var canvas = document.getElementById("myCanvas");
var ctx = canvas.getContext("2d");
ctx.moveTo(0,0);
ctx.lineTo(200,100);
ctx.stroke();
</script>
</body>
</html>
```
## Example Program
//<b>Drawing Circle</b>
```
<!DOCTYPE html>
<html>
<body>
<canvas id="myCanvas" width="200" height="100"
style="border:1px solid #d3d3d3;">
Your browser does not support the canvas element.
</canvas>
<script>
var canvas = document.getElementById("myCanvas");
var ctx = canvas.getContext("2d");
ctx.beginPath();
ctx.arc(95,50,40,0,2*Math.PI);
ctx.stroke();
</script> 
</body>
</html>
```
## Example Program
//<b>Creating Text</b>
```
<!DOCTYPE html>
<html>
<body>
<canvas id="myCanvas" width="200" height="100"
style="border:1px solid #d3d3d3;">
Your browser does not support the canvas element.
</canvas>
<script>
var canvas = document.getElementById("myCanvas");
var ctx = canvas.getContext("2d");
ctx.font = "30px Arial";
ctx.strokeText("Hello World",5,50);
</script>
</body>
</html>
```
## Example Program
//<b>Changing Text Color</b>
```
<!DOCTYPE html>
<html>
<body>
<canvas id="myCanvas" width="300" height="200"
style="border:1px solid #d3d3d3;">
Your browser does not support the canvas element.
</canvas>
<script>
var canvas = document.getElementById("myCanvas");
var ctx=canvas.getContext("2d");
ctx.font="30px Comic Sans MS";
ctx.fillStyle = "red";
ctx.textAlign = "center";
ctx.fillText("Hello World", canvas.width/3,canvas.height/2);
</script>
</body>
</html>
```








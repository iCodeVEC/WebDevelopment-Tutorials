# Javascript
JavaScript is the programming language of HTML and the Web.<br>
JavaScript is easy to learn.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<h1>My First JavaScript</h1>
<button type="button"
onclick="document.getElementById('demo').innerHTML = Date()">
Click me to display Date and Time.</button>
<p id="demo"></p>
</body>
</html>
```
## Why Study JavaScript?
JavaScript is one of the <b>3 languages</b> all web developers must learn:<br>
1. HTML to define the <b>content</b> of web pages.<br>
2. CSS to specify the <b>layout of web pages.</b><br>
3. JavaScript to program the <b>behaviour</b> of web pages.<br>
<b>NOTE:</b> JavaScript and Java are completely different languages, both in concept and design. 
JavaScript was invented by <b>Brendan Eich</b> in 1995, and became an <b>ECMA standard</b> in 1997.
<b>ECMA-262 is the official name of the standard.</b> 
<b>ECMAScript</b> is the official name of the language.
# Javascript Syntax
JavaScript syntax is the set of rules, how JavaScript programs are constructed.
## Javascript Programs
A computer program is a list of <b>instructions</b> to be executed by the computer.<br>
In a programming language, these program instructions are called <b>statements</b>.<br>
JavaScript is a <b>programming</b> language.<br>
JavaScript statements are separated by <b>semicolons</b> (;).
## Javascript Statements
JavaScript statements are composed of:<br>
1.Values<br>
2.Operators<br>
3.Expressions<br>
4.Keywords<br>
5.Comments
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<h1>JavaScript Statements</h1>
<p>Then the value of z is displayed in the paragraph below:</p>
<p id="demo"></p>
<script>
var x,y,z;
x = 5;
y = 6;
z = x + y;
document.getElementById("demo").innerHTML = z;
document.write(z);
window.alert(z);
console.log(z);
</script>
</body>
</html>
```
## Javascript Values
The JavaScript syntax defines two types of values: <b>Fixed values and variable values</b>.
Fixed values are called <b>literals</b>. Variable values are called <b>variables</b>.
## Javascript Literals
The most important rules for writing fixed values are:<br>
<b>Numbers</b> are written with or without <b>decimals.</b>
<b>Strings</b> are text, written within <b>double or single quotes.</b>
## Javascript Variables
In a programming language, variables are used to store <b>data values.</b><br>
JavaScript uses the <b>var</b> keyword to declare variables.<br>
An <b>equal sign</b> is used to assign values to variables.
## Javascript Operators
JavaScript uses <b>arithmetic operators ( + - *  / )</b> to compute values.
## Javascript Expressions 
An expression is a combination of values, variables, and operators, which computes to a value.<br>
The computation is called an evaluation.<br>
For example, 1 * 1 evaluates to 1.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p id="demo"></p>
<script>
document.getElementById("demo").innerHTML = "John" +" "+ "Doe";
</script>
</body>
</html>
```
## Javascript Keywords
JavaScript keywords are used to identify actions to be performed.<br>
The var keyword tells the browser to create variables.<br>
<b> JavaScript Is Case Sensitive</b>
## JavaScript and Camel Case
Historically, programmers have used three ways of joining multiple words into one variable name.<br>
<b>Hyphens:</b><br>
first-name, last-name, master-card, inter-city.<br>
Hyphens are not allowed in JavaScript. It is reserved for subtractions.<br>
<b><u>Underscore:<br></b></u>
first_name, last_name, master_card, inter_city.<br>
<b><u>Camel Case:<br></b></u>
FirstName, LastName, MasterCard, InterCity.<br>
JavaScript programmers tend to use camel case that starts with a lowercase letter.
## Identifiers
All JavaScript variables must be identified with <b>unique names.</b><br>
These unique names are called identifiers.<br>
The rules for legal names are much the same in most programming languages.<br>
•	Names can contain letters, digits, underscores, and dollar signs.<br>
•	Names must begin with a letter.<br>
•	Names can also begin with $ and _ (but we will not use it in this tutorial).<br>
•	Names are case sensitive (y and Y are different variables).<br>
•	Reserved words (like JavaScript keywords) cannot be used as names.
## Javascript Variables
JavaScript variables are containers for storing data values.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<h1>JavaScript Variables</h1>
<p>In this example, x, y, and z are variables</p>
<p id="demo"></p>
<script>
var x = 5;
var y = 6;
var z = x + y;
document.getElementById("demo").innerHTML = z;
</script>
</body>
</html>
```
## Javascript DataTypes
JavaScript variables can hold numbers like 100 and text values like "Hello World".<br>
In programming, text values are called text strings.<br>
JavaScript can handle many types of data, but for now, just think of numbers and strings.<br> 
Strings are written inside double or single quotes. Numbers are written without quotes.<br>
If you put a number in quotes, it will be treated as a text string.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<h1>JavaScript Variables</h1>
<p>Strings are written with quotes.</p>
<p>Numbers are written without quotes.</p>
<p>Try to experiment by removing the // comments.</p>
<p id="demo"></p>
<p id="demo1"></p>
<script>
var pi = 3.14+"person"+"answer";
var person = "Hello World";
var answer = 'Yes I am!';
document.getElementById("demo").innerHTML = pi;
document.getElementById("demo1").innerHTML = person;
document.getElementById("demo").innerHTML = answer;
</script>
</body>
</html>
```
## One Statement, Many Variables And Variable=undefined
You can declare many variables in one statement.<br>
Start the statement with var and separate the variables by <b>comma</b>.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<h1>JavaScript Variables</h1>
<p>You can declare many variables in one statement.</p>
<p id="demo"></p>
<p id="demo1"></p>
<script>
/*var person = "John Doe",
carName = "Volvo",
price = 200;*/
var person;
var person1=undefined;
var person="John Doe",carName="Volvo",price=200;
document.getElementById("demo").innerHTML = person;
document.getElementById("demo").innerHTML = person1;
document.getElementById("demo1").innerHTML = price;
</script>
</body>
</html>
```
## Re-Declaring JavaScript Variables
If you re-declare a JavaScript variable, it will not lose its value.<br>
The variable <b>carName</b> will still have the value <b>"Volvo"</b> after the execution of these statements.
## Example Program
```
<!DOCTYPE html>
<html>	
<body>
<h1>JavaScript Variables</h1>
<p>If you re-declare a JavaScript variable, it will not lose its value.</p>
<p id="demo"></p>
<script>
var carName = "Volvo";
var carName;
document.getElementById("demo").innerHTML = carName;
</script>
</body>
</html>
```
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<h1>JavaScript Variables</h1>
<p>The result of adding 5 + 2 + 3:</p>
<p id="demo"></p>
<script>
var x = 5 + 2 + 3;
document.getElementById("demo").innerHTML = x;
</script>
</body>
</html>
```
## Javascript Keywords
JavaScript statements often start with a keyword to identify the JavaScript action to be performed.<br>
Here is a list of some of the keywords you will learn about in this tutorial.
<table>
<tr>
<th>Keyword</th>
<th>Description</th>
</tr>
<tr>
<td>break</td>
<td>Terminates a switch or a loop</td>
</tr>
<tr>
<td>continue</td>
<td>Jumps out of a loop and starts at the top</td>
</tr>
<tr>
<td>debugger</td>
<td>Stops the execution of JavaScript, and calls (if available) the debugging function</td>
</tr>
<tr>
<td>do ... while</td>
<td>Executes a block of statements, and repeats the block, while acondition is true</td>
</tr>
<tr>
<td>for</td>
<td>Marks a block of statements to be executed, as long as a condition is true</td>
</tr>
<tr>
<td>function</td>
<td>Declares a function</td>
</tr>
<tr>
<td>if ... else</td>
<td>Marks a block of statements to be executed, depending on a condition</td>
</tr>
<tr>
<td>return</td>
<td>Exits a function</td>
</tr>
<tr>
<td>switch</td>
<td>Marks a block of statements to be executed, depending on different cases</td>
</tr>
<tr>
<td>try ... catch</td>
<td>Implements error handling to a block of statements</td>
</tr>
<tr>
<td>var</td>
<td>Declares a variable</td>
</tr>
<b>JavaScript programs (and JavaScript statements) are often called JavaScript code.</b>

























































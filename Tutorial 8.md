# Javascript Methods
JavaScript methods are the actions that can be performed on objects.<br>
A JavaScript method is a property containing a function definition.<br>
Methods are functions stored as object properties.<br>
<table>
<tr>
<th>Property</th>
<th>Value</th>
</tr>
<tr>
<td>First Name</td>
<td>John</td>
</tr>
<tr>
<td>Last Name</td>
<td>Doe</td>
</tr>
<tr>
<td>Age</td>
<td>50</td>
</tr>
<tr>
<td>Eye Color</td>
<td>Blue</td>
</tr>
<tr>
<td>Full Name</td>
<td>function() 
{return this.firstName + " " + this.lastName;}</td>
</tr>
</table>
# Accessing Object Methods
You create an object method with the following syntax:<br>
<b>methodName : function() { code lines }</b> <br>
You access an object method with the following syntax:<br>
<b>objectName.methodName()</b>
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p>Creating and using an object method.</p>
<p>A method is actually a function definition stored as a property value.</p>
<p id="demo"></p>
<p id="demo1"></p>
<script>
var person = {
    firstName: "John",
    lastName : "Doe",
    id       : 5566,
    fullName : function() {
       return this.firstName + " " + this.lastName;
    }
};
document.getElementById("demo").innerHTML = person.fullName();
document.getElementById("demo1").innerHTML=person.firstName+ " "+ person.lastName;
</script>
</body>
</html>
```
If you access the fullName property,without<b>()</b>,it will return the function definition.
# Using Built-In Methods
This example uses the `toUpperCase()` method of the String object, to convert a text to uppercase
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<script>
var message="Hello World!";
var x= message.toUpperCase();
document.write(x);
</script>
</body>
</html>
```
# Adding New Methods
Adding methods to an object is done inside the constructor function.
## Snippet
```
function person(firstName, lastName, age, eyeColor) {
    this.firstName = firstName;  
    this.lastName = lastName;
    this.age = age;
    this.eyeColor = eyeColor;
    this.changeName = function (name) {
        this.lastName = name;
    };
}
```
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p id="demo"></p>
<script>
function person(firstName,lastName,age,eyeColor) {
    this.firstName = firstName;
    lastName = lastName;
    //document.write(lastName);
    this.age = age;
    this.eyeColor = eyeColor;
    this.changeName = function (name) {
        this.lastName = name;
    }
}
var myMother = new person("Sally","Rally",48,"green");
myMother.changeName("Doe");
document.getElementById("demo").innerHTML =
"My mother's last name is " + myMother.lastName;
</script>
</body>
</html>
```
# Javascript Events
HTML events are "things" that happen to HTML elements.<br>
When JavaScript is used in HTML pages, JavaScript can "react" on these events.<br>
An HTML event can be something the browser does, or something a user does.
Here are some examples of HTML events:<br>
•	An HTML web page has finished loading<br>
•	An HTML input field was changed<br>
•	An HTML button was clicked<br>
Often, when events happen, you may want to do something.<br>
JavaScript lets you execute code when events are detected.<br>
HTML allows event handler attributes, with <b>JavaScript</b> code, to be added to HTML elements.<br>
With single quotes:<br>
`<some-HTML-element some-event='some JavaScript'>`<br>
With double quotes:<br>
`<some-HTML-element some-event="some JavaScript">`
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<button onclick="document.getElementById('demo').innerHTML=Date()">The time is?</button>
<p id="demo"></p>
</body>
</html>
```
# Changing  its own element:
The below  code changes the content of its own element (using this.innerHTML)
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<button onclick="this.innerHTML=Date()">The time is?</button>
<script>
document.write(Date());
</script>
</body>
</html>
```
##Event Handling Calling Functions:
## Example Program(Calling functions using event handling)
```
<!DOCTYPE html>
<html>
<body>
<p>Click the button to display the date.</p>
<button onclick="displayDate()">The time is?</button>
<script>
function displayDate() {
    document.getElementById("demo").innerHTML = Date();
}
</script>
<p id="demo"></p>
</body>
</html>
```
## Common HTML Events
Here is a list of some common HTML events:
<table>
<tr>
<th> Event </th>
<th> Description</th>
</tr>
<tr>
<td>onchange</td>
<td>An HTML element has been changed</td>
</tr>
<tr>
<td>onclick</td>
<td>The user clicks an HTML element</td>
</tr>
<tr>
<td>onmouseover</td>
<td>The user moves the mouse over an HTML element</td>
</tr>
<tr>
<td>onmouseout</td>
<td>The user moves the mouse away from an HTML element</td>
</tr>
<tr>
<td>onkeydown</td>
<td>The user pushes a keyboard key</td>
</tr>
<tr>
<td>onload</td>
<td>The browser has finished loading the page</td>
</tr>
</table>
## What can JavaScript Do?
Event handlers can be used to handle, and verify, user input, user actions, and browser actions:<br>
•	Things that should be done every time a page loads.<br>
•	Things that should be done when the page is closed.<br>
•	Action that should be performed when a user clicks a button.<br>
•	Content that should be verified when a user inputs data.<br>
•	And more ...<br>
Many different methods can be used to let JavaScript work with events:<br>
•	HTML event attributes can execute JavaScript code directly.<br>
•	HTML event attributes can call JavaScript functions.<br>
•	You can assign your own event handler functions to HTML elements.<br>
•	You can prevent events from being sent or being handled.<br>
•	And more ...<br>
# JAVASCRIPT FORM VALIDATION
HTML form validation can be done by JavaScript.
## Snippet
```
var i=document.form1.uname.value;
var a=i.length;
var j=document.form1.pass.value;
var b=j.length;
<form name="form1"><br>
Username<input type="text" name="uname"><br>
Password<input type="password" name="pass" onkeyup="passwordstrength(this.value)">
<label id="password description">Password not entered</label>
<input type="button"onclick="a()" value="submit">
</form>
```
## Validate of numbers
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<h1>JavaScript Can Validate Input</h1>
<p>Please input a number between 1 and 10:</p>
<input id="numb">
<button type="button" onclick="myFunction()">Submit</button>
<p id="demo"></p>
<script>
function myFunction() {
    var x, text;
// Get the value of the input field with id="numb"
    x = document.getElementById("numb").value;
    // If x is Not a Number or less than one or greater than 10
    if (isNaN(x) || x < 1 || x > 10) {
        text = "Input not valid";
    } else {
        text = "Input OK";
    }
    document.getElementById("demo").innerHTML = text;
}
</script>
</body>
</html>
```

























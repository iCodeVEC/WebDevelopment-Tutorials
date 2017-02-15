# Input Types in Html
This Tutorial describes the different input types for the `<input>` element.<br>
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<form action="action_page.php">
First name:<br>
<input type="text" name="firstname" maxlength="10" size="10">
<br>
Last name:<br>
<input type="text" name="lastname">
<br>
Password:<br>
<input type="password" name="pass"><br>
Gender:<br>
<input type="radio" name="gender" value="male" checked>Male<br>
<input type="radio" name="gender" value="female" >Female<br>
<input type="radio" name="gender" value="others" >Others<br>
Languages:<br>
 <select>
  <option>Select</option>
  <option value="tamil">Tamil</option>
  <option value="hindi">Hindi</option>
  <option value="english">English</option>
  <option value="french">French</option>
</select> <br>
<input type="checkbox">Agree&nbsp;
<input type="checkbox">Disagree<br>
<input type="text" name="firstname" value="nothing" disabled><br>
Read Only:<br><input type="text" name="firstname" value="nothing" readonly>
<br><input type="submit" value="Submit">
<input type="reset">
</form>
</body>
</html>
```
<b> NOTE:</b> For more information on `<input>` tag please refer to the following link:<br>
https://www.w3schools.com/html/html_form_input_types.asp
# Blocks in Html
A block-level element always starts on a new line and takes up the 
full width available (stretches out to the left and right as far as it can).<br>
## Examples of block-level elements:
1.`<div>`<br>
2.`<h1> - <h6>`<br>
3.`<p>`<br>
4.`<form>`<br>
## Inline Elements
An inline element does not start on a new line and only takes up as much width as necessary.<br>
## Examples of inline elements: 
1.`<span>`   
2.`<a>`<br>
3.`<img>`<br>
## The `<div>` Element:
The `<div>` element is often used as a container for other HTML elements.<br>
The `<div>` element has no required attributes, but both <b>style and class</b> are common.<br>
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<div style="background-color:black;color:white;margin:20px 0px 25px 15px;padding:20px;">
  <h2>London</h2>
  <p>London is the capital city of England.</p>
  <p>Standing on the River Thames,London looks Beautiful.</p>
</div> 
</body>
</html>
```
## The `<span>` Element:
The <span> element is often used as a container for some text.<br>
The <span> element has no required attributes, but both <b>style and class</b> are common.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<h1>My <span style="color:red; font-family:Monotype Corsiva">First</span>&nbsp;Class</h1>
</body>
</html>
```
# Class Attributes 
The HTML class attribute makes it possible to define equal styles for elements with the same class name.
## Example Program
```
<!DOCTYPE html>
<html>
<head>
<style>
div.cities {
    background-color: black;
    color: white;
    margin: 20px 30px 20px 30px;
    padding: 20px;
}
div.cities1 {
    background-color: black;
    color: red;
    margin: 20px 0 25px 0;
    padding: 1px;
}
div.cities2 {
    background-color: red;
    color: black;
    margin: 20px 0 15px 0;
    padding: 20px;
}
</style>
</head>
<body>
<div class="cities">
<h2>London</h2>
<p>London is the capital of England. It is the most populous city in the United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
<p>Standing on the River Thames, London has been a major settlement for two millennia, its history going back to its founding by the Romans, who named it Londinium.</p>
</div> 
<div class="cities1">
<h2>Paris</h2>
<p>Paris is the capital and most populous city of France.</p>
<p>Situated on the Seine River, it is at the heart of the Île-de-France region, also known as the région parisienne.</p>
<p>Within its metropolitan area is one of the largest population centers in Europe, with over 12 million inhabitants.</p>
</div>
<div class="cities2">
<h2>Tokyo</h2>
<p>Tokyo is the capital of Japan, the center of the Greater Tokyo Area, and the most populous metropolitan area in the world.</p>
<p>It is the seat of the Japanese government and the Imperial Palace, and the home of the Japanese Imperial Family.</p>
<p>The Tokyo prefecture is part of the world's most populous metropolitan area with 38 million people and the world's largest urban economy.</p>
</div>
</body>
</html>
```
<b>NOTE:</b> The HTML class attribute can also be used for inline elements (i.e) `<span>`tag
## Example Program
```
<!DOCTYPE html>
<html>
<head>
<style>
span.note {
    font-size: 120%;
    color: red;
}
span.note1
{
      font-size:50%;
      color:green;
}
span.note2
{
      font-size:150%;
      color:powderblue;
}

</style>
</head>
<body>
<h1>My <span class="note">Important</span> Heading</h1>
<p>This is some <span class="note1">important</span> text.</p>
<p> So please make a <span class="note2">note </span>of it.
</body>
</html>
```

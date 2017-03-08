#JavaScript Dates
The Date object lets you work with dates (years, months, days, hours, minutes, seconds, and milliseconds).
#JavaScript Date Formats
A JavaScript date can be written as a string<br>
<b>Mon Mar 06 2017 21:56:41 GMT+0530 (India Standard Time)</b><br>
or as Number<br>
<b>1488817601353</b><br>
Dates written as numbers, specifies the number of milliseconds since January 1, 1970, 00:00:00.
##Displaying Dates
In this tutorial we use a script to display dates inside a `<p>` element with `id="demo"`
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p id="demo"></p>
<script>
document.getElementById("demo").innerHTML = Date();
</script>
</body>
</html>
```
## Creating Date Objects
The Date object lets us work with dates.<br>
A date consists of a year, a month, a day, an hour, a minute, a second, and milliseconds.<br>
Date objects are created with the <b>new Date()</b> constructor.<br>
There are 4 ways of initiating a date:<br>
1)new Date()<br>
2)new Date(milliseconds)<br>
3)new Date(dateString)<br>
4)new Date(year, month, day, hours, minutes, seconds, milliseconds).<br>
Using new Date(), creates a new date object with the <b>current date and time</b>.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p id="demo"></p>
<script>
var d = new Date();
document.getElementById("demo").innerHTML = d;
</script>
</body>
</html>
```
Using new Date(date string), creates a new date object from the <b>specified date and time</b>.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p id="demo"></p>
<script>
var d = new Date("11:13:50 March 05, 2017");
document.getElementById("demo").innerHTML = d;
</script>
</body>
</html>
```
Using new Date(number), creates a new date object as <b>zero time plus the number</b>.<br>
Zero time is 01 January 1970 00:00:00 UTC. The number is specified in <b>milliseconds</b>.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p id="demo"></p>
<script>
var d = new Date(86400000);
document.getElementById("demo").innerHTML = d;
</script>
</body>
</html>
<!DOCTYPE html>
<html>
<body>
<p id="demo"></p>
<script>
var d = new Date(99,10,24,11,33,30,0);
document.getElementById("demo").innerHTML = d;
</script>
</body>
</html>
```
### Omitting Last Four Parameters:
```
<!DOCTYPE html>
<html>
<body>
<p id="demo"></p>
<script>
var d = new Date(99,5,24);
document.getElementById("demo").innerHTML = d;
</script>
</body>
</html>
```
## Date Methods
When a Date object is created, a number of methods allow you to operate on it.<br>
Date methods allow you to get and set the year, month, day, hour, minute, second, 
and millisecond of objects, using either local time or UTC (universal, or GMT) time.
## Displaying Dates
When you display a date object in HTML, it is automatically converted to a string, with the `toString()` method.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p id="demo"></p>
<script>
var d = new Date();
document.getElementById("demo").innerHTML = d.toString();
</script>
</body>
</html>
```
The `toUTCString()` method converts a date to a UTC string (a date display standard).
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p>The toUTCString() method converts a date to a UTC string (date display 
standard).</p>
<p id="demo"></p>
<script>
var d = new Date();
document.getElementById("demo").innerHTML = d.toUTCString();
</script>
</body>
</html>
```
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p id="demo"></p>
<script>
var d = new Date();
document.getElementById("demo").innerHTML = d.toDateString();
</script>
</body>	
</html>
```
# Time Zones
When setting a date, without specifying the time zone, JavaScript will use the browser's time zone.<br>
When getting a date, without specifying the time zone, the result is converted to the browser's time zone.<br>
In other words: If a date/time is created in GMT (Greenwich Mean Time), the date/time will be converted to 
CDT (Central US Daylight Time) if a user browses from central US.
## JavaScript Date Input
There are generally 4 types of JavaScript date input formats<br>
1)ISO Date-"2015-03-25" (The International Standard)<br>
2)Short Date-"03/25/2015"<br>
3)Long Date-"Mar 25 2015" or "25 Mar 2015"<br>
4)Full Date-"Wednesday March 25 2015"
## JavaScript Date Output
Independent of input format, JavaScript will (by default) output dates in full text string format<br>
Wed Mar 25 2015 05:30:00 GMT+0530 (India Standard Time).
## JavaScript ISO Dates
ISO 8601 is the international standard for the representation of dates and times.<br>
The ISO 8601 syntax (YYYY-MM-DD) is also the preferred JavaScript date format.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<h1>JavaScript ISO Dates</h1>
<p id="demo"></p>
<script>
document.getElementById("demo").innerHTML =
new Date("2015-03-25");
</script>
</body>
</html>
```
## ISO Dates (Year and Month)
ISO dates can be written without specifying the day (YYYY-MM)
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<h1>JavaScript ISO Dates</h1>
<p id="demo"></p>
<script>
document.getElementById("demo").innerHTML =
new Date("2015-03");
</script>
</body>
</html>
```
## ISO Dates (Only Year)
ISO dates can be written without month and day (YYYY)
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<h1>JavaScript ISO Dates</h1>
<p id="demo"></p>
<script>
document.getElementById("demo").innerHTML =
new Date("2015");
</script>
</body>
</html>
```
## ISO Dates (Date-Time)
ISO dates can be written with added hours, minutes, and seconds (YYYY-MM-DDTHH:MM:SSZ)<br>
Date and time is separated with a capital T.<br>
UTC time is defined with a capital letter Z.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<h1>JavaScript ISO Dates</h1>
<p>Separate date and time with a capital T.</p>
<p>Indicate UTC time with a capital Z.</p>
<p id="demo"></p>
<script>
document.getElementById("demo").innerHTML =
new Date("2017-03-07T02:00:00Z");
</script>
</body>
</html>
```
## JavaScript Short Dates
Short dates are written with an `"MM/DD/YYYY"` syntax like this
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p id="demo"></p>
<script>
document.getElementById("demo").innerHTML = new Date("03/25/2015");
</script>
</body>
</html>
```
## JavaScript Long Dates
Long dates are most often written with a `"MMM DD YYYY"` syntax like this
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p id="demo"></p>
<script>
document.getElementById("demo").innerHTML = new Date("Mar 25 2015");
</script>
</body>
</html>
```
<b>Month and day can be in any order.<br>
Commas are ignored. Names are case insensitive</b><br>
`var d = new Date("JANUARY, 25, 2015");`
## JavaScript Full Date
JavaScript will accept date strings in "full JavaScript format".
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p id="demo"></p>
<script>
document.getElementById("demo").innerHTML = 
new Date("Wed Mar 25 2015 09:56:24 GMT+0530 (India Standard Time)");
</script>
</body>
</html>
```
JavaScript will ignore errors both in the day name and in the time parentheses.
## JavaScript Date Methods
Date methods let you get and set date values (years, months, days, hours, minutes, seconds, milliseconds).
## Date Get Methods
<table>
<tr>
<th>Method</th>
<th>Description</th>
</tr>
<tr>
<td>getDate()</td>
<td>Get the day as a number (1-31)</td>
</tr>
<tr>
<td>getDay()</td>
<td>Get the weekday as a number (0-6)</td>
</tr>
<tr>
<td>getFullYear()</td>
<td>Get the four digit year (yyyy)</td>
</tr>
<tr>
<td>getHours()</td>
<td>Get the hour (0-23)</td>
</tr>
<tr>
<td>getMilliseconds()</td>
<td>Get the milliseconds (0-999)</td>
</tr>
<tr>
<td>getMinutes()</td>
<td>Get the minutes (0-59)</td>
</tr>
<tr>
<td>getMonth()</td>
<td>Get the month (0-11)</td>
</tr>
<tr>
<td>getSeconds()</td>
<td>Get the seconds (0-59)</td>
</tr>
<tr>
<td>getTime()</td>
<td>Get the time (milliseconds since January 1, 1970)</td>
</tr>
</table>
## Example Program to Display Month
```
<!DOCTYPE html>
<html>
<body>
<p>You can use an array to display the name of the weekday:</p>
<p id="demo"></p>
<script>
var d = new Date();
//var days = ["Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday"];
document.getElementById("demo").innerHTML = d.getDay();
</script>
</body>
</html>
```
## Date Set Methods
Set methods are used for setting a part of a date.<br>
The methods for setting date is same as that of getting dates except, instead of get set is used.<br>
For Example:<br>
setMonth().
## Snippets:
```
d.setDate(d.getDate() + 50);
d.setDate(20);
d.setFullYear(2020, 0, 14);
```
## Date Input - Parsing Dates
If you have a valid date string, you can use the Date.parse() method to convert it to milliseconds.<br>
Date.parse() returns the number of milliseconds between the date and January 1, 1970.
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p>Date.parse() returns the number of milliseconds between the date and January 1, 1970:</p>
<p id="demo"></p>
<script>
var msec = Date.parse("March 21, 2012");
var d=new Date(msec);
document.write(msec);
document.getElementById("demo").innerHTML = d;
</script>
</body>
</html>
```
## Compare Dates
Dates can easily be compared.<br>
The following example compares today's date with January 14, 2100
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p id="demo"></p>
<script>
var today, someday, text;
today = new Date();
someday = new Date();
someday.setFullYear(2100, 0, 14);
if (someday > today) {
    text = "Today is before January 14, 2100.";
} else {
    text = "Today is after January 14, 2100.";
}
document.getElementById("demo").innerHTML = text;
</script>
</body>
</html>
```
# JavaScript Strings
JavaScript strings are used for storing and manipulating text.<br>
A JavaScript string simply stores a series of characters like "Hello World".<br>
A string can be any text inside quotes. You can use single or double quotes.
## Strings Can be Objects
Normally, JavaScript strings are primitive values, created from literals: var firstName = "John"<br>
But strings can also be defined as objects with the keyword new: var firstName = new String("John").
## Example Program
```
<!DOCTYPE html>
<html>
<body>
<p id="demo"></p>
<script>
var x = "John";              // x is a string
var y = new String("John");  // y is an object
document.getElementById("demo").innerHTML =
typeof x + "<br>" + typeof y;
</script>
</body>
</html>
```
<b>Objects cannot be compared.</b>
##  String Properties and Methods
Primitive values, like "John Doe", cannot have properties or methods (because they are not objects).<br> 
But with JavaScript, methods and properties are also available to primitive values, 
because JavaScript treats primitive values as objects when executing methods and properties.
## String Properties
1)constructor-  Returns the string's constructor function <br>
2)length		 -  Returns the length of a string <br>
3)prototype	 -  Allows you to add properties and methods to an object
## String Methods
<table>
<tr>
<th>Method</th>
<th>Description</th>
</tr>
<tr>
<td>charAt()</td>
<td>Returns the character at the specified index (position)</td>
</tr>
<tr>
<td>charCodeAt()</td>
<td>Returns the Unicode of the character at the specified index</td>
</tr>
<tr>
<td>concat()</td>
<td>Joins two or more strings, and returns a new joined strings</td>
</tr>
<tr>
<td>endsWith()</td>
<td>Checks whether a string ends with specified string/characters</td>
</tr>
<tr>
<td>fromCharCode()</td>
<td>Converts Unicode values to characters</td>
</tr>
<tr>
<td>includes()</td>
<td>Checks whether a string contains the specified string/characters</td>
</tr>
<tr>
<td>indexOf()</td>
<td>Returns the position of the first found occurrence of a specified value in a string</td>
</tr>
<tr>
<td>lastIndexOf()</td>
<td>Returns the position of the last found occurrence of a specified value in a string</td>
</tr>
<tr>
<td>localeCompare()</td>
<td>Compares two strings in the current locale</td>
</tr>
<tr>
<td>match()</td>
<td>Searches a string for a match against a regular expression, and returns the matches</td>
</tr>
<tr>
<td>repeat()</td>
<td>Returns a new string with a specified number of copies of an existing string</td>
</tr>
<tr>
<td>replace()</td>
<td>Searches a string for a specified value, or a regular expression, and returns a new string where 
the specified values are replaced</td>
</tr>
<tr>
<td>search()</td>
<td>Searches a string for a specified value, or regular expression, and returns the position of the match</td>
</tr>
<tr>
<td>slice()</td>
<td>Extracts a part of a string and returns a new string</td>
</tr>
<tr>
<td>split()</td>
<td>Splits a string into an array of substrings</td>
</tr>
<tr>
<td>startsWith()</td>
<td>Checks whether a string begins with specified characters</td>
</tr>
<tr>
<td>substr()</td>
<td>Extracts the characters from a string, beginning 		
at a specified start position, and through the 	specified number of character</td>
</tr>
<tr>
<td>substring()</td>
<td>Extracts the characters from a string, between two specified indices</td>
</tr>
<tr>
<td>toLocaleLowerCase()</td>
<td>Converts a string to lowercase letters, according to the host's locale</td>
</tr>
<tr>
<td>toLocaleUpperCase()</td>
<td>Converts a string to uppercase letters, according to the host's locale</td>
</tr>
<tr>
<td>toLowerCase()</td>
<td>Converts a string to lowercase letters</td>
</tr>
<tr>
<td>toString()</td>
<td>Returns the value of a String object</td>
</tr>
<tr>
<td>toUpperCase()</td>
<td>Converts a string to uppercase letters</td>
</tr>
<tr>
<td>trim()</td>
<td>Removes whitespace from both ends of a string</td>
</tr>
<tr>
<td>valueOf()</td>
<td>Returns the primitive value of a String object</td>
</tr>
</table>
<b>NOTE:</b> All string methods return a new value. They do not change the original variable.<br>
## Snippet
Snippet:
```
//charAt();
function myFunction() {
    var str = "HELLO WORLD";
    var res = str.charAt(0)
    document.getElementById("demo").innerHTML = res;
}
```














                   











































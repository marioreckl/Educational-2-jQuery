# Variables

* We will provide an HTML file:
```html
<!DOCTYPE html>
<html lang="en-US">
<head>
  <meta charset="UTF-8">
  <title>Javascript Tutorial</title>
</head>
<body>
<button type="button">Click me!</button>
</body>
</html>
```
* We will add an `onlclick` event to the button and add the function between script tags in the body:
```html
<!DOCTYPE html>
<html lang="en-US">
<head>
  <meta charset="UTF-8">
  <title>Javascript Tutorial</title>
</head>
<body>
<button type="button" onclick="sayHello()">Click me!</button>

<script>
function sayHello() {
  alert("Hello, Reid!");
}
</script>
</body>
</html>
```
* Then, we'll take it up a notch and introduce variables.
```html
<!DOCTYPE html>
<html lang="en-US">
<head>
  <meta charset="UTF-8">
  <title>Javascript Tutorial</title>
</head>
<body>
<button type="button" onclick="sayHello()">Click me!</button>

<script>
function sayHello() {
  var name = prompt("Please enter your name");
  alert("Hello, " + name + "!");
}
</script>
</body>
</html>
```
* Since pressing Cancel results in the alert saying "Hello, null!" we can include an if statement:
```html
<!DOCTYPE html>
<html lang="en-US">
<head>
  <meta charset="UTF-8">
  <title>Javascript Tutorial</title>
</head>
<body>
<button type="button" onclick="sayHello()">Click me!</button>

<script>
function sayHello() {
  var name = prompt("Please enter your name");
  if (name != null) {
    alert("Hello, " + name + "!");
  }
}
</script>
</body>
</html>
```
* Addition of the confirm() option:
* 
```html
<!DOCTYPE html>
<html lang="en-US">
<head>
  <meta charset="UTF-8">
  <title>Javascript Tutorial</title>
</head>
<body>
<button type="button" onclick="sayHello()">Click me!</button>

<script>
function sayHello() {
var name = prompt("Please enter name: ")
if( name == null) {
      if(confirm("Are you sure you do not want to enter your name?") == false) {
            var name = prompt("Please enter name: ");
}
}
  
  if (name != null) {
    alert("Hello, " + name + "!");
  }
}
</script>
</body>
</html>
```
* Then, we'll take it up another notch and introduce arguments to replace the prompt.
```html
<!DOCTYPE html>
<html lang="en-US">
<head>
  <meta charset="UTF-8">
  <title>Javascript Tutorial</title>
</head>
<body>
<button type="button" onclick="sayHello('Reid')">Click me!</button>

<script>
function sayHello(x) {
  var name = x;
  alert("Hello, " + name + "!");
}
</script>
</body>
</html>
```

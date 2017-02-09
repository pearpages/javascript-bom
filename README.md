# The Browser Object Model (BOM)

> There are no official standards for the Browser Object Model (BOM).

Since modern browsers have implemented (almost) the same methods and properties for JavaScript interactivity, it is often referred to, as methods and properties of the BOM.

---

## The Window Object

Global variables are properties of the window object.

Global functions are methods of the window object.

```javascript
window.document.getElementById("header");

// is the same as:

document.getElementById("header");
```

### Window Size

> The browser window (the browser viewport) is NOT including toolbars and scrollbars.

* window.innerHeight - the inner height of the browser window (in pixels)
* window.innerWidth - the inner width of the browser window (in pixels)

### Other

* window.open() - open a new window
* window.close() - close the current window
* window.moveTo() -move the current window
* window.resizeTo() -resize the current window

---

## Window Screen

> The window.screen object contains information about the user's screen.

> The window.screen object can be written without the window prefix.

* screen.width
* screen.height
* screen.availWidth
* screen.availHeight
* screen.colorDepth
* screen.pixelDepth

### Screen availWidth

```javascript
document.getElementById("demo").innerHTML =
"Screen Width: " + screen.width;

// Result will be:

Screen Width: 2560
```

### Screen Height

```javascript
document.getElementById("demo").innerHTML =
"Screen Height: " + screen.height;
// Result will be:

Screen Height: 1080
```

### Screen Available Width

> The screen.availWidth property returns the width of the visitor's screen, in pixels, minus interface features like the Windows Taskbar.

```javascript
document.getElementById("demo").innerHTML =
"Available Screen Width: " + screen.availWidth;

//Result will be:

Available Screen Width: 2556
```

### Screen Available Height

```javascript
document.getElementById("demo").innerHTML =
"Available Screen Height: " + screen.availHeight;

//Result will be:

Available Screen Height: 1057
```

---

## Window Location

> The window.location object can be used to get the current page address (URL) and to redirect the browser to a new page.

The window.location object can be written without the window prefix.

* location.href   returns the href (URL) of the current page
* location.hostname   returns the domain name of the web host
* location.pathname   returns the path and filename of the current page
* location.protocol   returns the web protocol used (http: or https:)
* location.assign   loads a new document

```javascript
document.getElementById("demo").innerHTML =
"Page location is " + window.location.href;
```

```javascript
document.getElementById("demo").innerHTML =
"Page hostname is " + window.location.hostname;
```

```javascript
document.getElementById("demo").innerHTML =
"Page path is " + window.location.pathname;
```

```javascript
document.getElementById("demo").innerHTML =
"Page protocol is " + window.location.protocol;
```

### Location Assign

The window.location.assign() method loads a new document.

```javascript
<html>
<head>
<script>
function newDoc() {
    window.location.assign("http://www.w3schools.com")
}
</script>
</head>
<body>

<input type="button" value="Load new document" onclick="newDoc()">

</body>
</html>
```

---

## Window History

> The window.history object contains the browsers history.

* history.back() - same as clicking back in the browser
* history.forward() - same as clicking forward in the browser

```javascript
<html>
<head>
<script>
function goBack() {
    window.history.back()
}
</script>
</head>
<body>

<input type="button" value="Back" onclick="goBack()">

</body>
</html>
```

---

## Window Navigator

> The window.navigator object contains information about the visitor's browser.

* navigator.appName
* navigator.appCodeName
* navigator.platform

### Browser Cookies

The cookieEnabled property returns true if cookies are enabled, otherwise false.

```javascript
document.getElementById("demo").innerHTML =
"cookiesEnabled is " + navigator.cookieEnabled;
```

### Browser Application Name

The appName property returns the application name of the browser.

> Strange enough, "Netscape" is the application name for both IE11, Chrome, Firefox, and Safari.

```javascript
document.getElementById("demo").innerHTML =
"navigator.appName is " + navigator.appName;
```

### Browser Application Code Name

> "Mozilla" is the application code name for both Chrome, Firefox, IE, Safari, and Opera.

```javascript
document.getElementById("demo").innerHTML =
"navigator.appCodeName is " + navigator.appCodeName;
```

### The Browser Engine

The product property returns the product name of the browser engine:

```javascript
document.getElementById("demo").innerHTML =
"navigator.product is " + navigator.product;
```

### The Browser Version

```javascript
document.getElementById("demo").innerHTML = navigator.appVersion;
```

### The Browser Agent 

> The userAgent property returns the user-agent header sent by the browser to the server:

```javascript
document.getElementById("demo").innerHTML = navigator.userAgent;
```

### The Browser platform

The platform property returns the browser platform (operating system):

```javascript
document.getElementById("demo").innerHTML = navigator.platform;
```

### The Browser Language

The language property returns the browser's language.

```javascript
document.getElementById("demo").innerHTML = navigator.language;
```

### Is The Browser Online? 

```javascript
document.getElementById("demo").innerHTML = navigator.onLine;
```

### Is Java Enabled?

```javascript
document.getElementById("demo").innerHTML = navigator.javaEnabled();
```

---

## Window Popup Alert

---

## Window Timing

---

## Window Cookies

---
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
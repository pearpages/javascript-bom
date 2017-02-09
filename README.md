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


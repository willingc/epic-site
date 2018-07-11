---
title: "Project 5: Drawing"
date: 2018-07-10T18:08:30-07:00
anchor: "project5"
weight: 50
---

# Drawing

---

# Modern websites

In general:

- HTML :arrow_right: Structure
- CSS :arrow_right: Style
- JavaScript (`.js`) :arrow_right: interactivity

[codepen.io](https://codepen.io) to test code :bulb:

---

# `sketch.js` is a JavaScript file


**`sketch.js`**

```javascript
function setup() {
  // put setup code here
}

function draw() {
  // put drawing code here
}
```

---

# `index.html`

```html, [.highlight: 7, 10]
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=0>
    <style> body {padding: 0; margin: 0;} </style>
    <script src="../p5.min.js"></script>
    <script src="../addons/p5.dom.min.js"></script>
    <script src="../addons/p5.sound.min.js"></script>
    <script src="sketch.js"></script>
  </head>
  <body>
  </body>
</html>
```

---

# Canvas

The canvas coordinates are different than in math class.
- top left `(0,0)`
- bottom right `(width-1, height-1)`

```javascript
createCanvas(300, 100);  // Canvas width is 300 pixels, height is 100 pixels
```

For example:
- top left `(0,0)`
- bottom right `(299, 99)`

---

# Draw an ellipse and circle

```javascript
ellipse(centerPixelsFromLeft, centerPixelsFromTop, width, height);
```

*Example*

[.code: auto(42), line-height(2.0)]

```javascript, [.highlight: 6-7]
function setup() {
  createCanvas(400, 400);
}

function draw() {
  ellipse(150, 90, 20, 20);  // Draw a circle (width=height)
  ellipse(200, 200, 80, 10); // Draw an ellipse
}
```

---

# Draw more shapes

```javascript, [.highlight: 6-10]
function setup() {
  createCanvas(400, 400);
}

function draw() {
  ellipse(150, 90, 20, 20);  // Draw a circle (width=height)
  ellipse(200, 200, 80, 10); // Draw an ellipse
  line(0, 0, 50, 50);
  rectangle(300, 200, 50, 30);
  rectangle(50, 70, 30, 30);
}
```

---

# Explore

- Change values
- Add a shape
- Run examples

---

# Drawing

- Learn about HTML, CSS, JS files
- Understand canvas
- Code a shape
- Code multiple shapes

Completed

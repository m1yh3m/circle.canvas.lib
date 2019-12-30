# circle.canvas.lib

Library for creating canvas circle

### usage

```javascript
const Circle = require("@m1yh3m/circle.canvas.lib");
```

### a complete example

[jsfiddle](https://jsfiddle.net/jshacker/Lu3up6j0/)

```javascript
var canvas = document.getElementById("canvas");
var context = canvas.getContext("2d");

var c = new Circle(); // import it from somewhere

c.in(context)
  .fillWith("maroon")
  .of(20)
  .fillAt(300, 300)
  .fillAt(260, 260)
  .fillWith("teal")
  .fillAt(28, 28)
  .of(38)
  .fillWith("navy")
  .fillAt(100, 100);

var d = new Circle();
d.in(context)
  .fillWith("lime")
  .of(23)
  .fillAt(30, 300);

var e = new Circle();
e.in(context)
  .drawWith({ strokePattern: "black", lineWidth: 4 })
  .of(10)
  .drawAt(300, 30)
  .drawWith({ strokePattern: "blue", lineWidth: 3 })
  .of(20)
  .drawAt(300, 20)
  .drawWith({ strokePattern: "magenta", lineWidth: 2 })
  .of(30)
  .drawAt(300, 50)

  .drawWith({ strokePattern: "black", lineWidth: 5 })
  .of(30)
  .drawAt(300, 140)
  .of(27)
  .fillWith("yellow")
  .fillAt(300, 140);
```

```html
<canvas id="canvas" height="400" width="400"></canvas>
```

```css
canvas {
  outline: thin solid #333;
}
```

## copied from

https://github.com/gitfaf/canvas-js

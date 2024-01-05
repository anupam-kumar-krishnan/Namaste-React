# _Namaste React⚛️_
## _Episode 03 Part 02 🚀_

## _React Element_ ⚛️
- React Element is not an HTML element
- **`React.createElement`** => at the end of the day is an <b>Object</b>
- And when we render this **`element`** onto DOM, it becomes a **`HTML element`**

<b>

```js
const heading = React.createElement("h1", {id: "heading"}, "Namaste React 🚀");
```
</b>

## _Not Rendered_
- If something goes wrong, then we write for better practice/understanding `Not Rendered` inside div root

<b>

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <link rel="stylesheet" href="./index.css" />
  <body>
    <div id="root"><h1>Not Rendered</h1></div>
    <script type="module" src="./App.js"></script>
  </body>
</html>
```
<b>




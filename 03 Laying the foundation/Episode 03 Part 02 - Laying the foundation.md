# _Namaste React⚛️_
## _Episode 03 Part 02 🚀_

## _React Element_ ⚛️
- React Element is **_not_** an **_HTML element_**
- <b>`React.createElement` => `Object` => `HTMLElement`</b>
- **`React.createElement`** -> at the end of the day is an <b>_`Object`_</b>
- And when we render this **`element(React.createElement)`** onto DOM, it becomes a **`HTML element`**


<b>

```js
const heading = React.createElement(
   "h1",
   {id: "heading"},
   "Namaste React 🚀"
);

const root = ReactDOM.createRoot(document.getElementById("root"));

root.render(heading);
```
</b>

## _Not Rendered_
- Anytime in your app, **`Not Rendered`** displaying on the screen that means there is a problem with your **`render`**. Also it is a better practice/understanding.

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




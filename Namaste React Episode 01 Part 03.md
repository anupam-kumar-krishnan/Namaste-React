# _Namaste React EP 01 Part 03_ 🚀

Now separate the file in HTML and JavaScript

## _index.html_

<b>

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Namaste React</title>
  </head>
  <body>
    <div id="root"></div>
    <script
      crossorigin
      src="https://unpkg.com/react@18/umd/react.development.js"
    ></script>
    <script
      crossorigin
      src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"
    ></script>
    <script src="./app.js"></script>
  </body>
</html>
```

## _app.js_

```javascript
const heading = React.createElement("h1",{},"Hello World from React JS!!");
const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(heading);
```

## _Attributes_

```javascript
const heading = React.createElement(
"h1",
 {id: "heading", xyz:"abc"},
"Hello World from React JS!!"
);
const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(heading);
```

</b>




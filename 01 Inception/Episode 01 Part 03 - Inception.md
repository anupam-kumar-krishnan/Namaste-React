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

`{}` - _this object is the place where you will give attributes to your tags_

### _Suppose_
- If we need to give attribute to a class or element say h1 here, we can give in object is id

```javascript
const heading = React.createElement(
  "h1",
  {id:"heading"},
  "Hello World from React JS!!"
);
```

## _Attributes_

```javascript
const heading = React.createElement( // here heading is an object
"h1",
 {id: "heading", xyz:"abc"},  // attributes
"Hello World from React JS!!" // children
);

console.log(typeof heading); //object

const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(heading); 
//this render method is responsible to take this object(heading here) and convert in tag and put it up in DOM
```

`props` - props are children + the attributes that we pass

Here, props are-
```javascript
{id: "heading", xyz:"abc"},
"Hello World from React JS!!"
```
</b>

## _What is the most costly operation in webpage?_
- The most costly operation in webpage is **_when the DOM nodes needs to be manipulated._**
- Putting somes nodes in the DOM, removing some nodes from the DOM(operation)
- And all these frameworks & libraries are coming to optimise this
- React comes with a philosophy, that whatever is needed to be done in a webpage, do it in javascript<br>
   (i.e. Manipulting the DOM using JavaScript)








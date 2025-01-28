# _Namaste React Episode 01 Part 02_ 🚀

- After writing Hello World using plain HTML, using plain Javascript and after ejecting React JS, We are now writing the same using **_React JS_**

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


    <script>
      const heading = React.createElement(
        "h1",
        {},
        "Hello World from React JS!!"
      );
      const root = ReactDOM.createRoot(document.getElementById("root"));
      root.render(heading);
    </script>
  </body>
</html>
```
</b>




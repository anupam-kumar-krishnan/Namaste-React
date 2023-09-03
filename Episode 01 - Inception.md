# _Namaste React EP1_ 🚀
- A JavaScript Library, not a Framework

### _Episode 1_

_Before Starting_
1. Make Notes
2. Use Laptop - Learn and Apply the same
3. Maintain a GitHub Repository

### _Tools_
- Google Chrome(Developer Console)
- VS Code

### _Small Recap of HTML, CSS and JS_
- Hello World

### _Homework_
- CDN
- Crossorigin

### _Simple Hello World in HTML5_
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
    <div id="root">
    <h1>Hello World!</h1>
    </div>
  </body>
</html>
```
</b>

### _Hello World Using JavaScript_
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
   <script>
     const heading = document.createElement("h1");
     heading.innerHTML = "Hello World from JavaScript!";
     const root = document.getElementById("root");
     root.appendChild(heading);
   </script>
  </body>
</html>
```
</b>

### _Hello World Using React JS_

- First, get React into the project
- Get React by using CDN(Content Delivery Network)
- CDN: These are the website where particular codes are hosted and we are just pulling that code into our project

### _HTML5_


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
   <script crossorigin 
    src="https://unpkg.com/react@18/umd/react.development.js">
   </script> // Core of React
   <script crossorigin 
    src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"> 
   </script> //React Library for DOM Operations
   <script src="./app.js"></script>
  </body>
</html>
```

### _app.js_

```js
 const heading = document.createElement("h1");
 heading.innerHTML = "Hello World from JavaScript!";
 const root = document.getElementById("root");
 root.appendChild(heading);
```



</b>


### _Use React in HTML5_

Why there are two file?

- First file is Core of React
- Second file is the react library for DOM Operations

React just not work on browsers, but mobiles too i.e. React-native

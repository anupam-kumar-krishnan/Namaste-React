# _Namaste React EP01 P04_ 🚀

### _How will you create this type of structue in React?_
- Object is the ReactElement
- ReactElement(Object) becomes => HTML(that browser understands)


<b>


```html
<div id="parent">
     <div id="child">
         <h1>I'm H1 tag</h1>
     </div>
</div>
```
```javascript
const parent = React.createElement(
 "div",
 { id: "parent" },
 React.createElement(
  "div",
  { id: "child" },
    React.createElement("h1", {}, "I'm H1 tag")
 ) 
);
```

</b>

## _How to create siblings in React?_

<b>

```html
<div id="parent">
     <div id="child">
         <h1>I'm H1 tag</h1>
         <h2>I'm H2 tag</h2>
     </div>
</div>
```
```javascript
const parent = React.createElement(
 "div",
 { id: "parent" },
 React.createElement("div",{ id: "child" }, [
    React.createElement("h1", {}, "I'm H1 tag"),  // array of children
    React.createElement("h2", {}, "I'm H2 tag"),  // array of children
 ]) 
);
```


</b>








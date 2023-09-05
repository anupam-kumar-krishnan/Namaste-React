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

```javascript
<div id="parent">
     <div id="child">
         <h1>I'm H1 tag</h1>
         <h2>I'm H2 tag</h2>
     </div>
<div id="child"2>
         <h1>I'm h1 tag</h1>
         <h2>I'm h2 tag</h2>
       </div>
</div>
```

```javascript
const parent = React.createElement("div", { id: "parent" }, [
   React.createElement("div", { id: "child" ), [
    React.createElement("h1", {}, "I'm an h1 tag"),
    React.createEement("h2", {}, "I'm an h2 tag"),
   ]),
    React.createElement("div", { id: "child2" ), [
    React.createElement("h1", {}, "I'm an h1 tag"),
    React.createEement("h2", {}, "I'm an h2 tag"),
  ]),
]);
```

<b><i>

## _Important_
- Now, one must be thinking that its very tough to write siblings like this, but the motive of react was to make code easy for us right, that's why JSX has been intoduced

- JSX will make our life easy, when it comes to making tags
</i></b>

## _Note_

<b><i>
- Now, we will no longer be using createElement
- We will learn React 18 stuff
</i></i>


</b>








# _Namaste React⚛️_
## _Episode 03 Part 04 🚀_

## _React Components⚛️_
- _**Everything is a Component in React JS**_

### _There are two types of components in React JS⚛️_
- **_Class Based Component_** (OLD Way)
- **_Functional Component_** (NEW Way)

## _React Funtional Component_
- It is just a normal _**JavaScript Function**_ which returns some piece of _**JSX**_
- A JavaScript Function which returns a _**React Element**_ is a **_Functional Component_**
- Name the function with a **_CAPITAL_** letter otherwise we will get an error (This is React way to understand this is a component)

<b>

```js
//React Functional Component
const HeadingComponent = () => {
    return <h1>Namaste React Functional Component</h1>
};
```
</b>

## _Functional Component with and without `return`_
### _Without return_
- When you have just only line in funtion, then you can just skip this `return`

<b>

```js
const fn = () => true
```
```js
const HeadingComponent = () => <h1>Namaste React Functional Component</h1>;
```

## _With return_

```js
const fn2 () => {
  return true;
};
```
```js
const HeadingComponent = () => (
 return <h1>Namaste React Functional Component</h1>;
);
```

## _Perfectly valid Functional Component_
- _We can write like this_

```js
const HeadingComponent = () => (
 <div id="container"> 
     <h1>Namaste React Functional Component</h1>;
 </div>
);
```

## _How we will render `Component` inside `root`_

```js
const HeadingComponent = () => (
 <div id="container"> 
     <h1>Namaste React Functional Component</h1>;
 </div>
);

root.render(<HeadingComponent />); 
// Babel Understands a functional component like this
```

## _Component Composition:_
-  _Write Component inside Component_

```js
const Title = () => (
  <h1 cllassName="head" tabIndex="5">
    <h1>Namaste React Using JSX🚀</h1>
   </h1>

const HeadingComponent = () => (
 <div id="container">
  <Title /> //Component
  <h1 className="heading">Namaste React Functional Component</h1>
  </div>
); 

const root = ReactDOM.createRoot(document.getElementById("root"));

root.render(<HeadingComponent />);
```

</b>











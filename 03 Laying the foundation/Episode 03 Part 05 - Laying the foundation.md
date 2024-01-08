# _Namaste React⚛️_
## _Episode 03 Part 05 🚀_

## _Functional Component can be created normally using function_
- It's not mandatory to use **`Arrow Function`**
- But **`Arrow Function`** is a **`Industry Wide Standard`**

<b>

```js
const Title = function () {
return (
  <h1 className="head" tabIndex="5">
    Namaste React using JSX 🚀
  </h1>
  );
};
```
</b>

## _Element inside a Component_

## _Superpower of JSX_
- In JSX, if you write a **`curly braces`** anywhere inside **`JSX`**, inside this curly braces, you can run any piece of **`JavaScript Expression`**

<b>

```js
const number = 10000,

const HeadingComponent = () => (
  <div id="container">
     {number}
     <h1 className="heading">Namaste React Functional Component</h1>h1>
  </div>

const root = ReactDOM.createRoot(document.getElementById("root"));

root.render(<HeadingComponent />);
```
</b>

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

## _Superpower of JSX_ 🔮🪄
- In JSX, if you write a **`curly braces`** anywhere inside **`JSX`**, inside this curly braces, you can run any piece of **`JavaScript Expression`**

<b>

```js
const number = 10000,

const HeadingComponent = () => (
  <div id="container">
     {number}
     <h1 className="heading">Namaste React Functional Component</h1>
  </div>

const root = ReactDOM.createRoot(document.getElementById("root"));

root.render(<HeadingComponent />);
```
</b>


## _React Element inside a Component_

<b>

```js
const title = (
   <h1 className="head" tabIndex="5">
      Namaste React Using JSX 🚀
    </h1>
);

const HeadingComponent = () => (
  <div id="container">
     {title}
     <h1 className="heading">Namaste React Functional Component</h1>
  </div>
);

const root = ReactDOM.createRoot(document.getElementById("root"));

root.render(<HeadingComponent />);
```
</b>

## _Security🔐 in JSX_
- JSX escapes the **_Malicious Data_**
- It will sanitize the data and then pass it
- It prevents **_Cross-Site Attacks_** for you

## _Ways of writing React Element or Component inside another Componet_

<b>

```js
const Title = () => (
  <h1 className="head" tabIndex=5">
     Namaste React using JSX 🚀
  </h1>
);

const HeadingComponent = () => (
  <div id="container">
     <Title></Title> // or <Title /> like this
     <h1 className="heading">Namaste React Functional Component</h1>
  </div>
);

const root = ReactDOM.createRoot(document.getElementById("root"));

root.render(<HeadingComponent />);
```
</b>

## _What I can call inside a Component_
- _**JavaScript Expression**_
- _**Function**_
- _**Component**_

## _How can I write inside a Component_
- _**Inside Curly Braces**_ **`{Title()}`**
- _**Component**_ **`<Title />`**
- _**Another way of writing Component**_ **`<Title></Title>`**










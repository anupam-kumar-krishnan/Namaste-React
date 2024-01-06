# _Namaste React⚛️_
## _Episode 03 Part 03 🚀_

## _React Element_
- It's not very **developer friendly**, it's very **hard** to read also
- It looks very clumsy

<b>

```js
const heading = React.createElement(
 "h1",
 {id: "heading"},
 "Namaste React 🚀"
);
```
</b>

## _JSX_
- To help all the developers, Facebook developers created something known as _**JSX**_
- JSX is a syntax which is easier to create React Elements
- JSX is **NOT** a part of **_REACT_**
- We can build large applications without using JSX also, but JSX makes developers life easy
- JSX is a convention where we kind of merge these HTML and CSS together
- **_JSX is not HTML, JSX is HTML like or XML like syntax_**
- JSX is not reactElement, _**reactElement is an object**_ while _**JSX is a syntax**_

## _Create a heading(h1) tag using JSX_

<b>

```jsx
const jsxHeading = <h1>Namaste React using JSX 🚀</h1>;
```
</b>

## _**⚠️Important Note:⚠️**_ 
- _**JSX is not HTML written inside JavaScript**_
- **_JSX is not HTML, JSX is HTML like Syntax or XML like_**

### _React element using core React VS React element using JSX_
<b>

```js
const heading = React.createElement(
 "h1",
 {id: "heading"},
 "Namaste React 🚀"
);
```

VS

```jsx
const jsxHeading = <h1 id="heading">Namaste React using JSX 🚀</h1>;
//This looks much cleaner than the above using Core React
```

## _We will never be using React.createElement😮‍💨_ _Use JSX 😌_
</b>



## _Is the below code a valid JavaScript?🤔💭_
- This is not a valid Pure JavaScript
- JavaScript doesn't come with JSX built inside it
- JS Engine doesn't understand JSX


<b>

```jsx
const jsxHeading = <h1>Namaste React using JSX 🚀</h1>;
```
</b>

## _JS Engine doesn't understand JSX. Why?_
### > _JS Engine understands **`Ecmascript`**_

## _If JS Engine doesn't understand this, then how this code is working?_
### > _`Parcel` is doing the job behind the scenes_

## ‼️ _How the code is Working⚛️? 🤔💭_

_**Answer:**_
- _**When we write JSX code, the code is `transpiled` before it reaches to the JS Engine.
Then JS Engines receives the code that browsers can understand**_
- _**Transpiling** is done by **Parcel**_
- _Also **`Parcel`** is not doing all **alone**, **`Parcel`** gives this reponsibility of **`transpilation`** to **`Babel`**_
- _**`Parcel`** installs **`Babel`**_
- **`Babel`** is a JavaScript compiler that converts modern JavaScript code into a version compatible with all browsers.
- Babel's job is to transform **`JSX`** to **`React`** code


![working of jsx code](https://github.com/anupam-kumar-krishnan/Namaste-React/assets/69143883/702df916-c9bb-49f9-9fa6-a0e57e352b96)


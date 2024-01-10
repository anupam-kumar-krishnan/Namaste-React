# _Namaste React⚛️_
## _Episode 04 Part 02 🚀_

### _How to make components Dynamic?_
# _Props_
- Short form of _**Properties**_
- Props at the end of the day are just normmal **_arguments_** to a function
- **_"Passing a prop to a function is just like passing an argument to a function"_**

<b>

```js
<ResturantCard
 resName="Meghana Foods"
 cuisine="Biryani, North Indian, Asian"
/>
```
</b>

Here, the props are _**resName**_ and _**cuisine**_

## _How to use Props_
- Here, Props is an Object
- We all know that we can write any javascript code inside curly braces `{}`
- Objects are accessed by using `dot(.)` with the Parameter i.e. `props.resName`

<b>

```js
const RestaurantCard = (props) => {
  console.log(props);
  return (
    <div className="res-card" style={styleCard}>
      <img
        className="res-logo"
        alt="res-logo"
        src="https://media-assets.swiggy.com/swiggy/image/upload/fl_lossy,f_auto,q_auto,w_660/89fccaa76f2f760e2742b9e53d32bb69"
      />
      <h3>{props.resName}</h3>
      <h4>{props.cuisine}</h4>
      <h4>4.4 Stars</h4>
      <h4>38 mins</h4>
    </div>
  );
};
```

## _Destructuring on the fly_

_**Destructuring on the fly means**_

```js
const ResturantCard = ({resName, cuisine}) => {
  return (
    <div className="res-card" style={styleCard}>
      <img
        className="res-logo"
        alt="res-logo"
        src="https://media-assets.swiggy.com/swiggy/image/upload/fl_lossy,f_auto,q_auto,w_660/89fccaa76f2f760e2742b9e53d32bb69"
      />
      <h3>{resName}</h3>
      <h4>{cuisine}</h4>
      <h4>4.4 Stars</h4>
      <h4>38 mins</h4>
    </div>
  );
};

```



_Earlier_

```js
const RestaurantCard = (props) => {
const { resName, cuisine } = props;
  return (
    <div className="res-card" style={styleCard}>
      <img
        className="res-logo"
        alt="res-logo"
        src="https://media-assets.swiggy.com/swiggy/image/upload/fl_lossy,f_auto,q_auto,w_660/89fccaa76f2f760e2742b9e53d32bb69"
      />
      <h3>{props.resName}</h3>
      <h4>{props.cuisine}</h4>
      <h4>4.4 Stars</h4>
      <h4>38 mins</h4>
    </div>
  );
};
```





</b>









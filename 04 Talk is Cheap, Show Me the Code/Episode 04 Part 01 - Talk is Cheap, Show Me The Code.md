# _Namaste React⚛️_
## _Episode 04 Part 01 - Talk is Cheap, Show Me The Code🚀_

# _Building Food🍚🍜 Ordering App_
### _Planning_
- You should exactly know,what you are going to build 
- In the planning comes the UI Design

## _Components of Food Ordering App_

### _Header_
   - Logo
   - Nav Items
### _Body_
   - Search
   - ResturantContainer
      - ResturantCard
### _Footer_
   - Copyrights
   - Links
   - Address
   - Contact

## _Inline Styles in React_
- Written like an object
- Inline Styles is not prefered way to write code


<b>

```js
const styleCard = {
  backgroundColor: "yellow"
}

const ResturantCard = () => {
  return (
    <div className="res-card" style={styleCard}>
      <h3>Meghna Foods</h3>
    </div>
  );
};
```
OR

## _Why we write two bracket here_
- First bracket is to tell, there is some piece of `JavaScript` insde it
- Second braket is the `JavaScript Object`


```js
const ResturantCard = () => {
  return (
    <div className="res-card" style={{
       backgroundColor: "yellow"
     }}>
      <h3>Meghna Foods</h3>
    </div>
  );
};
```

</b>






 






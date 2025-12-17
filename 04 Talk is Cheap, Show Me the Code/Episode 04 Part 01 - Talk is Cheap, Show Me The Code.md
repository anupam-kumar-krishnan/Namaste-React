# _Namaste React⚛️_
## _Episode 04 Part 01 - Talk is Cheap, Show Me The Code🚀_

# _Building Food🍚🍜 Ordering App_
### _Planning_
- You should exactly know,what you are going to build 
- In the planning comes the UI Design

## _Components of Food Ordering App_

![Food UI](https://github.com/anupam-kumar-krishnan/Namaste-React/assets/69143883/5c5734fb-5552-415c-af0c-7c1cf32644c8)

<img width="829" height="947" alt="image" src="https://github.com/user-attachments/assets/a67eb685-270a-423e-a3f2-a638eeb01e72" />


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






 






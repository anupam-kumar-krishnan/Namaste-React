# _Namaste React EP1 Part 05_ 🚀

In the previous parts, we have ejected react using two files i.e. <b><i>Core of React JS</b></i> and <b><i>React DOM</b></i>

### _But, will the order of these two files matter?_
<b>


```html
<script src="./app.js"></script>
<script
      crossorigin
      src="https://unpkg.com/react@18/umd/react.development.js">
</script>
<script
      crossorigin
      src="https://unpkg.com/react-dom@18/umd/react-dom.development.js">
</script>
```
</b>


![react error](https://github.com/anupam-kumar-krishnan/Namaste-React/assets/69143883/40cdd062-4251-4be1-8ab3-fe062a10fc24)

As seeen above, if we write the <b>`<script src="./app.js"></script>`</b>, this will throw an error saying <b>`React`</b> is <b>`not defined`</b>



**_Note: The order of these files are always in sequence_**

## _Root.render(parent)_
- It is puting that parent inside the root tag
- But if something is already there in the id, then it will be **replaced** the content from there to concent placed in render.
- It is replaced **_very fast_** 🚀
- Whatever is rendered, it is rendered inside the root and rest remains the same

## _Library VS Framework: What React is Library or Framework?_
- We call <b>`React JS`</b> as library because React can be applied to a <b>`small portion`</b> of a page itself 
- React JS can work <b>`independently`</b> in a <b>`small portion of your app`</b> as well
- Not all frameworks can be applied to an existing app, but you can just React and start using in a small portion 
- This is why <b>`React JS`</b> is a library.










 


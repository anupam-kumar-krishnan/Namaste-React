# _Namaste React_ ⚛️🚀
## _Episode 03 Part 01_

### _Command to create a development built_
<b>

```js
npx parcel build index.html // development build
```
</b>


## _Scripts to build our Project_
- The commands are different for development build and production build
- To make our life easier, we create a script that will build our project instead of writing this command again and again
- It's a standard convention in the industry to build our scripts
- We need to create the script in _**package.json**_


### _How to create Scripts_
- _**In Package.json,**_ write under scripts:

<b>

```js
"scripts": {
  "start": "parcel index.html",
  "build": "parcel build index.html",
},
```
</b>

### _How to run these Scripts_
 
**_Start Project Locally:_** 
<b>

 ```js
 npm run start OR npm start
 ``` 
</b>


**_Build for Prouction:_**
<b>

 ```js
 npm run build
 ``` 
</b>














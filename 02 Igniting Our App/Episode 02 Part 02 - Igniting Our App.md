# _Igniting Our App_ ⚛️
## _Episode 02 Part 02_ 🚀

### _Running the server using Parcel_
<b>

```js
npx parcel index.html
```
</b>

## _npx_
- Just like we have npm, we have something known as npx
- **npx** means _**Executing a Package**_

## _Parcel📦_ 
- Parcel goes to the index.html and builds a development build for our app. <br>And it host that development build to our localhost:1234

## _Ways to get React into our app_
- Via _**Content Delivery Network(CDN)**_ <br>(This is not a prefered way to bring react and react-dom)
- Via npm

## _install react as a package_
<b>

```js
npm install react
```
</b>

## _Install React⚛️ as a Package. But Why?🤔💭_
- Fetching from CDN takes a costly operation, it will a network call to unpkg.com and it will get React from unpkg.com
- Suppose if I already have React in my node_modules, how easy it would it be to use React in our code
- We don't make another network call to get React, we will already have in our node modules
- Suppose another version of React comes in future, so we have to keep change the version of React in CDN link. 
- So it's better to have it in our package.json, it is easier to manage all our dependencies, it is very easy to manage React also as one of the dependenies inside our npm package.json
- Now we will install React as a Package in our code

## _If we remove the CDN Links_
- Then it will throw an error that <b>`React is not defined`</b>
- And it will display only what is there in HTML, not the content which id rendered in React(as we have removed the CDN links & also we have just installed react but not used it i.e. imported React JS)

## _[Now]: Import React from Node modules_

```js
import React from "react";
```

- Here, this react basically refers to the react inside our node module
- Similarly we will import react-dom from our node_modules


```js
import React from "react";
import ReactDOM from "react-dom";
```

- Now, will the code work? It shows an error, `browser scripts cannot have imports & exports`
- What does `browser scripts cannot have imports & exports` mean
- In HTML, we are ejectng App.js, so it treats this script as a browser script. It treats this is a normal javascript file (normal javaScript does not have import in it), but in actual it is not

## _Make browser understand that the file App.js is not a normal file_
- This is why, we need to tell browser about the file which is not a normal file, it's a module
- To make browser understand, add <b>`type=module`</b> in script tag

```js
<script type=module" src="./App.js"></script>
```

- Now, React is not coming from the CDN link, but from the dependency which we have installed(from node_modules)

## _Warning_ ⚠️

```js
Warning: You are importing createRoot from "react-dom" which is not supported. You should instead import it from "react-dom/client".
```

- Now this warning will be coming in console
- To overcome this error, write 

```js
import ReactDOM from "react-dom/client"
```

- And the warning will be gone

## _Magic🪄_ _Automatically Refershing of Page_
- This is done by the use of **`"Parcel"`**

## _Parcel_ 📦 
- Dev Build
- Local Server
- Hot Module Replacement(HMR) (Auto Refershing)
- How Parcel does this Auto Refresh? <br>Parcel uses a file watching algorithm - written in C++
- Caching - Faster Builds⚒️<br>
_**If we build subsequently, it will reduce the time, as it is caching things up**_
   - Where it is Caching things up? 
      - In .parcel-cache folder
- Image Optimization
- Minification
- Bundling
- Compress
- Consistent Hashing
- Code Splitting
- Differential Bundling - support older browser
- Diagnostic
- Error Handling
- Tree Shaking - remove unused code for you
- HTTPs
  - **_Suppose I want to test something which only works in https(SSL), Parcel gives you that feature also_**
- Different dev and prod bundles

## _Production built using Parcel_ 📦

<b>

```js
npx parcel build index.html
```
</b>

- Note: remove the main: "App.js" from package.json as there the entry point is App.js but we are running index.html
- All the Production built goes inside **_dist folder_**
- It takes time to build production built(1.4s) while parcel took 431ms

## _Note:_
- _**.parcel-cache**_ and _**dist**_ are Temporary folders, they can be regenerated

## _Browserslist_ 🔮🪄
[BrowsersList Website](https://browserslist.dev/)

- Tell your project that what all browsers should your app be supported in
- You have to configure it in package.json
- Use Case of browserslist: In Case of Government Websites, it should work on the oldest versions too(have 99% of browser coverage)
<b>

```js
"browserslist": [
    "last 2 Chrome version",
    "last 2 Firefox version"
 ]
```
</b>

## _We have built our own create-react-app⚛️ in this episode✨💫🌟🌠_



























































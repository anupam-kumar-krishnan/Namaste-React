# _Igniting Our App 🚀_
### _Episode 02 Part 01_

## _What Igniting Our App means?_
- We have written code in <b>`HTML`, `CSS` and `JS`</b>, but is this code ready to Production? NO right
- This code is **not** **`fully optimiszd`, `random comments coming`, `console.logs`** etc.
- We want to minify our code, we want to bundle our code
- To make your code ready to **`production`**, you need a lot of **`processing in your local`**/ or a lot of processing before you put the code to production
- You need to basically do <b>`bundling`</b>, <b>`code spliting`</b>, <b>`chunking`</b>, <b>`compressing`</b> before you can make your code go to production

## _Can React alone make a production ready app?_
- **_No Right_**. There are a lot of packages, JavaScript code that somebody has written makes our app fast to an extent but alot of packages are needed


## _How you can make your production readdy app? <br>(without using npx create-react-app)_

## _What is not NPM?_
- NPM is everything, but not **`Node Package Manager`**
- NPM doesn't have a full form
- NPM manages packages but it does not stand for  **`Node Package Manager`**

## _What NPM actually is?_
- NPM is a Standard repository for all the packages
- Any package you need to include in your project, you use NPM
- All packages are hosted over there

### **_Note:_** _Package.json is a configuraion for NPM_

## _Why do we need this package.json?_
- Our project is dependent on a lot of packages, those pakages with the project are dependent on the dependencies and NPM manages that
- NPM will take care of the version of that package
- **_package.json is a configuration for NPM_**
- **_Package_** and **_dependency_** are same


## _The most important package: Bundler_
- Bundler basically bundles your app, packages your app properly so that it can be shipped to production

## _Some of Bundler:_
- Webpack
- Parcel
- Vite

## **_Note_**
- When we write **`create-react-app`**, behind the scenes uses **_Webpack Bundler_**

## **_Parcel_**
We will be using **`Parcel`** Bundler


## **_There are two types of dependencies:_**
### _Dev Dependencies_
- It is generally required in a deveopment phase

#### _Normal Dependencies_
- Normal Dependencies are used in production

## _Caret(^) in package.json_
- If you install a package with latest version today and tommorow a new version comes in
- Then what will happen if you have put this caret, that package will automatically be upgraded to the latest version.
- It will install minor versions automatically

## _Tilde(~) in package.json_
- It will install major version automatically





















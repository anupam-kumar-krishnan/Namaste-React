# _Igniting Our App 🚀_
### _Episode 02 Part 01_

## _What Igniting🔥 Our App means?_
- We have written code in <b>`HTML`, `CSS` and `JS`</b>, but _**"Is this code ready to push to Production?"**_ _**NO right**_
- _**What is the issue in this code?**_ 🤔💭 This code is **not** **`fully optimized`, `random comments`, `console.log`** etc.
- We want to _**minify our code**_, we want to _**bundle**_ our code
- If we have a lot of images, we have to _**optimize those images**_
- To make your code ready to **`production`**, you need a lot of **`processing in your local`**/ or a lot of processing before you put the code to production
- You need to basically do <b>`bundling`</b>, <b>`code spliting`</b>, <b>`chunking`</b>, <b>`compressing`</b> before you can make your code go to **`production`**

## _Suppose you have to build⚒️ a fast production ready app and Can React⚛️ alone make a production ready app🏃‍♂️🚩?_
- **_No Right_**. There are a lot of packages that are required to make our production ready app, lot of JavaScript code that somebody has written makes our app fast to an extent but alot of packages are needed
- React is making app fast but to an extent, there are lot of other things we need to make our app fast, a lot of packages are required

## _How you can make your production ready app? <br>(without using npx create-react-app)<br> How we can get those packages in our app_

## _❌ What is not NPM?_
- NPM is everything, but not **`Node Package Manager`**
- NPM _**doesn't**_ have a _**full form**_
- NPM manages packages but it does not stand for  **`Node Package Manager`**

## _✅ What NPM actually is?_
- NPM is a Standard repository for all the packages
- Any package you need to include in your project, you use NPM
- All packages are hosted over there

## **_🍁 Note:_** _Package.json is a configuration for NPM_

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
- It is generally required in a **_development phase_**

### _Normal Dependencies_
- Normal Dependencies are used in **_production_**

## _Caret(^) in package.json_
- If you install a package with latest version today and tommorow a new version comes in
- Then what will happen if you have put this caret, that package will automatically be upgraded to the latest version.
- It will install **_"Minor Versions Automatically"_**
- It is always safe to put Caret to update the minor versions but not tilde as a major upgrade may break a lot of things in the app

## _Tilde(~) in package.json_
- It will install **_"Major Version Automatically"_**

## ⚠️ _Important: Caret(^) vs Tilde(~)_

## ‼️ _Important Points:_
### _package.json_
- When we install any package, dev dependencies were added in **_package.json_**
- **_package.json_** keeps a track of what version in installed in your system
- It keeps the **_approx version_** of packages
- _**package.json**_ is a _**configuration for NPM**_


### _package-lock.json_
- But we also got another file named **_package-lock.json_**
- **_package-lock.json_** keeps the exact version which is being installed
- It kind of locks the version and keeps the record of it
- It keeps the **_exact version_** of packages

### _shash2 in parcel (package-lock.json)_
- Have you herd that sometimes, code works on local but breaks on production
- It keeps the shash that whatever is in my dev machine, is the same version which is being deployed onto the production.

### _Difference: package.json VS package-lock,json_

## _Node Modules_
- It contains all the code that we fetched from **_NPM_**
- It has _**actual data of dependencies**_ that our project needs and that's why it is **_Huge_**

## _Transitive dependency_
A transitive dependency is one not imported directly into the project at hand, but instead imported by a direct dependency or another transitive dependency. 

## _Should Ipush all these node_modules code to GitHub_
- The answer is absolutely **_NO_**.
- So what we will do is, we will put this node_modules inside `.gitignore` file
- `.gitignore:` If you want something to not go on Github, just put inside `.gitignore` file




















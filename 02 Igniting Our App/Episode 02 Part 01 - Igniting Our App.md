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

## _Bundler_
Bundlers are essential tools in modern web development, particularly when working with frameworks like React. They are responsible for taking various files (JavaScript, CSS, images, etc.) within a React application and combining them into a single or a few optimized bundles for deployment.

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
> `^` allows both minor and patch updates while keeping the major version fixed, whereas `~` allows only patch updates while keeping both major and minor versions fixed.

### _In Short:_ `Caret allows minor and patch updates, whereas tilde allows only patch updates.`

## Difference between Caret(^) and Tilde(~)

| Feature                  | Caret (`^`)                    | Tilde (`~`)                 |
| ------------------------ | ------------------------------ | --------------------------- |
| Purpose                  | Allows safe feature updates    | Allows only small bug fixes |
| Updates Allowed          | ✅ Minor + Patch                | ✅ Patch only                |
| Major Version Change     | ❌ Not allowed                  | ❌ Not allowed               |
| Minor Version Change     | ✅ Allowed                      | ❌ Not allowed               |
| Patch Version Change     | ✅ Allowed                      | ✅ Allowed                   |
| Example                  | `^18.2.0`                      | `~18.2.0`                   |
| Can Install              | 18.2.1, 18.3.0                 | 18.2.1, 18.2.9              |
| Cannot Install           | 19.0.0                         | 18.3.0                      |
| Stability                | Medium                         | High                        |
| Flexibility              | High                           | Low                         |
| Common Usage in React    | Most libraries (react, router) | Strict APIs, utilities      |
| Risk of Breaking Changes | Low                            | Very Low                    |


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

### _sha512 in parcel (package-lock.json)_
- Have you herd that sometimes, code works on local but breaks on production
- It keeps the shash that whatever is in my dev machine, is the same version which is being deployed onto the production.

### _Difference: package.json VS package-lock.json_

| Feature                      | `package.json`                               | `package-lock.json`                                    |
| ---------------------------- | -------------------------------------------- | ------------------------------------------------------ |
| Purpose                      | Defines project metadata & dependency ranges | Locks the **exact versions** of all installed packages |
| Created By                   | Developer (manual or auto)                   | Automatically generated by npm                         |
| Editable                     | ✅ Yes                                        | ❌ No (should not be manually edited)                   |
| Defines Version Type         | ✅ Uses ranges (`^`, `~`)                     | ✅ Uses exact versions                                  |
| Controls Dependency Versions | ❌ Indirectly                                 | ✅ Directly                                             |
| Tracks Sub-Dependencies      | ❌ No                                         | ✅ Yes (full dependency tree)                           |
| Required for App Setup       | ✅ Yes                                        | ✅ Yes (for consistent installs)                        |
| Used in Production           | ✅ Yes                                        | ✅ Yes                                                  |
| Affects Install Consistency  | ❌ May vary across machines                   | ✅ Guarantees same output everywhere                    |
| Performance Impact           | ❌ None                                       | ✅ Speeds up install                                    |
| Risk Without It              | Version mismatch bugs                        | ❌ No major risk                                        |
| Should Be Pushed to Git?     | ✅ Yes                                        | ✅ Yes                                                  |
| File Size                    | Small                                        | Larger                                                 |
| Example                      | `"react": "^18.2.0"`                         | `"react": "18.2.0"`                                    |


## _Node Modules_
> `node_modules` is the directory that contains all installed npm packages required by a React application, including both direct and indirect dependencies.

- It contains all the code that we fetched from **_NPM_**
- It has _**actual data of dependencies**_ that our project needs and that's why it is **_Huge_**

### Why Is node_modules So Huge?

Because it includes:

- Your dependencies
- Their dependencies
- And their dependencies… <br>
  ➡️ This creates a deep dependency tree

## _Transitive dependency_
A transitive dependency is one not imported directly into the project at hand, but instead imported by a direct dependency or another transitive dependency. 

## _Should I push all these node_modules code to GitHub?🤔💭_
- The answer is absolutely **_NO_**.
- So what we will do is, we will put this node_modules inside **`.gitignore`** file
- **`.gitignore:`** If you want something to not go on Github, just put inside **`.gitignore`** file

## _Should I push package.json and package-lock.json on GitHub?🤔💭_
- The answer is absolutely **_YES_**
- `package.json` and `package-lock.json` maintains a note of what all dependencies the project needs
- Now you understand why `package-lock.json` is huge, it is basically maintaining the exact version of each dependency

## _Why we don't push node modules to GitHub?🤔💭_
- If you have _**package.json**_ and _**package-lock.json**_, you can recreate all your _**node modules**_ 




























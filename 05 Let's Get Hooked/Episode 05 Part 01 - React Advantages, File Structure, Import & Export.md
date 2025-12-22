# Episode 05 Part 01 - React Advantages, File Structure, Import & Export

### Why we are using React?
- Whatever we make can be also built by using normal HTML, CSS, JS or any other Library or framework
- At the end of the day, React is also JavaScript

### Reason
- We are using React because it makes the Developer Experience (DX) easy
- It makes you write less code and do more on the webpage
- This is the major job of a UI Library of a Framework is
- So React gives us super-powers so that we can make large scale, production ready, performant applications.
- React mekes our coding experience very fast and also otimises on ebpage so that things happen very fast

<hr/>

## React File Structure
- Place every single component in one single file named 'components'
- The filename should start with capital alphabet

- src
  - components
    - Header.js
    - HeroSection.js
    - RestaurantCard.js
    - MobileSection.js
    - Footer.js 

## Import & Export
- Once we have moved these componenets in single file, we have to first export every single component
- And then to use, we need to import the same
- First Export then Import
- We can ignore the file extension while importing the component
- Never keep hardcoded data (APIs) in components folder

### Types pf Export/Import
- Named
  - Export: `export const Component`
  - Import: `import {Component} from "path";`
- Default
  - Export: `export default Component`
  - Import: `import Component from "path";`

- Note:
  -  Wherever we have named export like CON_URL, we have to write it in curly braces while importing
  -  Default exports need not to be written inside curly braces

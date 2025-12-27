## What is a Hook?
Hook is nothing but a normal JavaScript function which React gives to us.

## What is `useEffect` in React JS?
useEffect is a React Hook used to handle side effects in functional components.

useEffect gets called, _**after the component has been rendered**_.

**👉 _Side effects are tasks that happen outside rendering, such as:_**
- Fetching data from an API
- Updating the DOM
- Subscribing/unsubscribing to events
- Timers (setTimeout, setInterval)
- Logging, analytics

<br> 

useEffect will be helpful when we implenent the second approach of data fetching.

**Loads > Render > API > Re-render**

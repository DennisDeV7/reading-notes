# Putting It All Together

## Thinking in React

[Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

1. What is the single responsibility principle and how does it apply to components?\
The single responsibility principle is the idea that a component should only be doing one thing.
2. What does it mean to build a ‘static’ version of your application?\
A static version of your application is one that does not change data via state it simply passes data via props
3. Once you have a static application, what do you need to add?\
Once you have a static applicatino you then need to add interactivity through state
4. What are the three questions you can ask to determine if something is state?
    1. Is it passed in from parent via props? If so, it is not in state.
    2. Does it remain unchanged over time? If so, it probably isn't state.
    3. Can you compute it based on any other state or props in your component? If so, it isn't state.
5. How can you identify where state needs to live?\
You can identify where state needs to live by following these steps:

- Identify every component that renders something based on that state.
- Find a common owner component (a single component above all the components that need the state in the hierarchy).
- Either the common owner or another component higher up in the hierarchy should own the state.
- If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

## Higher-Order Functions

[Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

1. What is a “higher-order function”?\
A higher-order function is one that operates on other functions by taking them as arguments of by returning them
2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?\
Line 2 of the function is creating another function that can determine if a new number is greater than the originally entered number.
3. Explain how either map or reduce operates, with regards to higher-order functions.
The map method builds a new array after applying a function to all of the elements of the original array. The reduce method builds a value by combining single elements of an array with its current value.

## Class Notes

```js
let numbers = [1, 2, 3, 4, 5];

let totalSum = numbers.reduce((runningTotal, currentValue) => {
  return runningTotal + currentValue;
}, 0)

console.log(totalSum); //15

let strArr = ['b', 'a', 'n', 'a', 'n', 'a', 's'];

let newStrArr = strArr.reduce((runningStr, currentValue) => {
  return runningStr + currentValue;
}, '');

console.log(newStrArr); // bananas
```

## Things I want to know more about

# State and Props

## React Lifecycle

what happens first, the 'render' or the componentDidMount?

What is the very first thing to ahppen in the lifecycle of React?

Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

What does componentDidMount do?

## Video State Vs Props

1. What types of things can you pass in the props?
2. What is the big difference between props and state?
3. When do we re-render our application?
4. What are some examples of things that we could store in state?

## Class

```js
'use strict'

let arr = [1,2,3,4];
let strArr = ['one', 'two', 'three', 'four'];

let newArr = arr.map(num => num * 5);
console.log(newArr); // [5,10,15,20]

let newStrArr = strArr.map(str => str.toUpperCase());
console.log(newStrArr); // ['ONE', 'TWO', 'THREE', 'FOUR']

// below will do the same thing as the map function above excep map does more work for you.
let newStrArr2 = [];
strArr.forEach(str => {
  newStrArr2.push(str.toUpperCase());
})
console.log(newStrArr2); // ['ONE', 'TWO', 'THREE', 'FOUR']


```

When an in state element is changed it will reload the render function

### Ternary

```js
let BoolValue = true

if (BoolValue) {
  console.log('it is true');
} else {
  console.log('it is false');
}

// Ternary
// What? true: false

BoolValue ? true : false;
```

## Things I want to learn more about

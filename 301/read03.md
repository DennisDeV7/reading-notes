# Passing Functions as Props

## React Docs - lists and keys

[React Docs](https://reactjs.org/docs/lists-and-keys.html)

1. What does `.map()` return?\
Map returns an array of equal length.
2. If I want to loop through an array and display each value in JSX, how do I do that in React?\
In React by simply putting the variable in curly brackets you can display each value in JSX. See example from React Docs.

  ```js
  const numbers = [1, 2, 3, 4, 5];
  const listItems = numbers.map((number) => 
    <li>{number}</li>
  );
  ```

3. Each list item needs a unique___.\
Each list item needs a unique key
4. What is the purpose of a key?\
"Keys help React identify which items have changed, are added, or are removed" (React Docs)

## Spread Operator

[Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b)

1. What is the spread operator?\
An ellipsis of three dots which expands an array into a list of arguments
2. List 4 things that the spread operator can do.

- Copy an array
- Concatenate arrays
- Use Math functions
- Add an items to a list

3. Give an example of using the spread operator to combine two arrays.\

From (Spread Operator)

```js
const hello = {hello: "😋😛😜🤪😝"}
const world = {world: "🙂🙃😉😊😇🥰😍🤩!"}

const helloWorld = {...hello,...world}
console.log(helloWorld) // Object { hello: "😋😛😜🤪😝", world: "🙂🙃😉😊😇🥰😍🤩!" }
```

4. Give an example of using the spread operator to add a new item to an array.

From (Spread Operator)

```js

const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍
```

5. Give an example of using the spread operator to combine two objects into one.

```js
const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂
```

## How to Pass Functions Between Components

1. In the video, what is the first step that the developer does to pass functions between components?\
Create a new function that calls that passes in the function
2. In your own words, what does the increment function do?\
The increment function takes in the array 'people' and returns a new array 'ppl' with an updated 'count' key value pair
3. How can you pass a method from a parent component into a child component?\
Pass it as if it were a prop.
4. How does the child component invoke a method that was passsed to it from a parent component?\
Create the prop such as `this.props.increment(this.props.name)`

## Class

### Filter

```js
'use strict';

let arr = [1,2,3,4,5,6,7,8];

let newArr = arr.filter(num => num > 4);

console.log (newArr); // [5,6,7,8]

let strArr = ['cat', 'mouse', 'dog'];

let newStrArr = strArr.filter(str => str.length === 3);

console.log(newStrArr);
```

## Things I Want to Learn More About

map functions\
spread operators\
passing functions between components

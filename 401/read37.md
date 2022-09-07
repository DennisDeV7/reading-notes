# React 1

## Overview

declare a variable: `let x = 0`

declare a constant: `const x = 0`

arrow function: `let func = a => {}`

template literal: `let str = "release date: ${date}`

method definintion shorthand:

```js
var obj = {
    a: function (c, d) {},
    b: function (e, f) {},
}
```

Array iteration:

```js
var arr = ['a', 'b', 'c']
for (var i=0, i < arr.length; i++) {
    console.log(arr[i])
}
```

Spread:

```js
let arr1 = [1, 2, 3]
let arr2 = ['a', 'b', 'c']
let arr3 = [...arr1, ...arr2]

console.log(arr3) // [1, 2, 3, 'a', 'b', 'c']
```

## React

JSX: JavaScript extension, produces React elements by combining rendering logic with user interface logic

In order to render an element you first have to pass the DOM element to ReactDOM.createRoot(), then pass the element to root.render()

Reace component:

```js
class Welcome extends React.Component {
    render() {
        return <h1>Hello, {this.props.name}</h1>;
    }
}
```

## Tailwind CSS

Tailwind uses utlity classes to build custom designs directly in HTML without a separate CSS file

example:

```html
<div class="p-6 max-w-sm mx-auto bg-white rounded-xl shadow-lg flex items-center space-x-4">
  <div class="shrink-0">
    <img class="h-12 w-12" src="/img/logo.svg" alt="ChitChat Logo">
  </div>
  <div>
    <div class="text-xl font-medium text-black">ChitChat</div>
    <p class="text-slate-500">You have a new message!</p>
  </div>
</div>
```

## Next.js

Create a Next.js app:

`npx create-next-app nextjs-blog --use-npm`

you can also use the `--exmaple` flag followed by a url to use a template

Run development server:

1. cd into project
2. npm run dev

## Things I want to learn more about
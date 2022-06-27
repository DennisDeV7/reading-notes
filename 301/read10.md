# In memory storage

## JavaScript Call Stack

1. What is a ‘call’?\
A call is a term to describe invoking a function.
2. How many ‘calls’ can happen at once?\
Functions are executed one at a time.
3. What does LIFO mean?\
LIFO means last in, first out when describing how data is stored and retrieved.
4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.\

5. What causes a Stack Overflow?

## JavaScript error messages

1. What is a ‘reference error’?
2. What is a ‘syntax error’?
3. What is a ‘range error’?
4. What is a ‘tyep error’?
5. What is a breakpoint?
6. What does the word ‘debugger’ do in your code?

## Class

```js
'use strict';

let array2D = [
  ['D', 't', 'ab', 'B'],
  ['o', 'a', 'o', 'r'],
  ['n\'', 'l', 'u', 'u'],
  ['t', 'k', 't', 'no']
]
for (let i in array2D) {
  let str = '';
  for (let j in array2D[i]){
    str += array2D[j][i];
  }
  console.log(str); // Don't talk about bruno
}

```

## Things I want to know more about
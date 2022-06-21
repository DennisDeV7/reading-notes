# Node.js

## Intro to Node.js

[Node.js on sitepoint.com](https://www.sitepoint.com/an-introduction-to-node-js/)

1. What is node.js?\
Node.js is a asynchronous event-driven JavaScript runtime. 
2. In your own words, what is Chrome’s V8 JavaScript Engine?\
The v8 JavaScript Engine is an open source software that compliles JavaScript to machine code that a computer can execute
3. What does it mean that node is a JavaScript runtime?\
The runtime means that it enables the computer to execute JavaScript code.
4. What is npm?\
NPM or node package manager is a package manager that helps download millions of available JavaScript software packages
5. What version of node are you running on your machine?\
I am running version 18.0.0 of node.
6. What version of npm are you running on your machine?\
I am running version 8.6.0 of npm on my computer.
7. What command would you type to install a library/package called ‘jshint’?\
`npm install -g jshint`
8. What is node used for?
Node is used to automate the process of developing a modern JavaScript application

## Pair Programming

[6 Reasons for Pair Programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)

1. What are the 6 reasons for pair programming?

    1. Greater efficiency
    2. Engaged collaboration
    3. Learning from fellow students
    4. Social skills
    5. Job interview readiness
    6. Work enviornment readiness
2. In your experience, which of these reasons have you found most beneficial?\ In my experience I found that it helps greatly with efficiency. Having another person observing and helping can help fill in gaps of knowledge, keep you on topic, and research in the background if you get stuck to help things go way faster.
3. How does pair programming work?\
In pair programming one person is the "driver" and is physically typing out the code. The other person is observing and guiding the driver to write the correct code and researching necessary topics to make the typer more efficient.

## Class

```js
'use strict';

let cat = 'cat';
let copyCat = cat;
console.log('cat', cat); // cat cat
console.log('copyCat', copyCat); // copyCat cat

copyCat = 'Boots';
console.log('cat' , cat); // cat cat
console.log('copyCat', copyCat); // copyCat Boots

let pets = ['Fido', 'Spot', 'Sparky'];
let copyPets = pets;
console.log('pets', pets); // pets ['Fido', 'Spot', 'Sparky']
console.log('copyPets', copyPets); // copyPets ['Fido', 'Spot', 'Sparky']

copyPets.push('Buddy');
console.log('pets', pets); // pets ['Fido', 'Spot', 'Sparky', 'Buddy']
console.log('copyPets', copyPets); // copyPets ['Fido', 'Spot', 'Sparky', 'Buddy']
// They are the same because copyPets is just a reference to the real array so if you push something to copyPets it is pushing it to the real array which is pets
// We must use an spread function to genuinely copy an array
let realCopyPets = [...pets];

```

## Things I want to learn more about
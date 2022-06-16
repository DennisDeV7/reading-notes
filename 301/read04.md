# React and Forms

## Forms

1. What is a ‘Controlled Component’?\
A controlled component is one that displays an item but also controls what the item does on subsequent user input.
2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.\
In order for it to be a controlled component i think it would have to update their response as soon as they enter them. This will give it the ability to pass it to other UI elements or reset it from another event handler.
3. How do we target what the user is entering if we have an event handler on an input field?\
By updating the setState as the information is input

## The Conditional (Ternary) Operator Explained

1. Why would we use a ternary operator?\
We would use a ternary operator in order to shorten certain if loops.
2. Rewrite the following statement using a ternary statement:

```js
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
```

Rewritten with ternary statement

```js
x === y ? true: false;
```

## Class Notes

## Things I want to learn more about


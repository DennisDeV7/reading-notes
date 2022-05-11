# Read 3 Notes

## Chapter 3: Lists

There are three types of lists in HTML:

1. Ordered Lists

    - created with the `<ol>` element
    - contains individual list items within it: `<li>`
    - used to display a list sequentially with numbers

2. Unordered Lists

    - created with the `<ul>` element
    - contains individual list items within it: `<li>`
    - displays a list of items in bullet format order does not matter

3. Definition Lists

    - created with the `<dl>` element
    - can contain definition terms, `<dt>`, or different definition, `<dd>`
    - this helps display a series of terms and their corresponding definition.

## Chapter 13: Boxes

- Control dimensions of a box

  - height: 300px;  ---> just a simple declaration in the style
  - width: 200px;
  - min-width: 200px; ---> can help contain a paragraph so it does not appear to thin in a large screen.
  - max-width: 300px;
  - min-height: 10px;
  - max-height: 20px;
  - overflow: hidden;
  - overflow: scroll;

- Create a border around a box

  - border: thin;
  - border: thick;
  - border: medium;
  - border: top-width; ---> one for other sides as well
  - border-style: solid; ---> see below for list of additional styles
    - dotted
    - dashed
    - double
    - groove
    - ridge
    - inset
    - outset
  - border-color: blue;
  - border: 4px dotted black; ---> thickness, style, and color in one property

- Set margins and padding for boxes

  - padding: 5px;
  - padding-top: 4px; ---> one for other directions as well
  - margin: 20px;
  - margin-top: 20px; ---> one for other directions as well

- Show and hide boxes

  - text-align: center; ---> centers a box
  - display: inline;
    - block
    - inline-block
    - none
  - visibility: hidden;
    - visible;
  - border-image: ---> page 319
  - box-shadow:
  - border-radius:

## JS Chapter 2: JS Instructions

A script is a series of instructions that JavaScript gives the web browser. Each individual script is called a statement. It may be necessary at times to declare variables. A variable allows you to assign a value to a keyword. A variable consists of a keyword, a name, an assignment operator, and the value. An array is a variable that can store more than one value.

## JS Chapter 4: Decisions and Loops

- flowchart: helps display the flow of logic so it is easier to code
- if statements: if a condition is evaluated as true than it executes the code in the body
- if else:
- switch: statement that contains many cases of possible values for a variable (switch value). If the variable matches the value than the corresponing code is executed.
- Truthy: values treated as if they are true
- Falsy: values treated as if they are false
- Short circuit values: returns a value that stopped or caused  "short circuit" in the logical operator
  [Table of Contents](README.md)
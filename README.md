# 30DaysJS
30 Days of JavaScript

## Project 1

This project I learned about data-* attributes, which allows the storage of custom information on HTML elements. 

The data attributes can be accessed via CSS and JavaScript, which make them very useful.

Data-*
https://developer.mozilla.org/en-US/docs/Learn/HTML/Howto/Use_data_attributes

#### Example
Adding data- before the value makes it into a data attribute
     <div data-name="snare" data-key="74" class="key">
      <kbd>J</kbd>
      <span class="sound">snare</span>
    </div>

 JavaScript Access
    let key = document.querySelector(`.key[data-key=65]`)
    ket.dataset.name // "snare"

CSS access
    div[data-name='snare']{
        width: 400px;
        background: red;
    }

Event Listener 'transitionend' used to listen for when a CSS transition has finished it's transition was something I found very useful as well.

## Project 2

I learned to use the Date() function and utilizing the different methods to make the clock hands move based on the getSeconds(), getMinutes(), and getHours() for each clock hand respectively.

Date()
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date

setInterval()
https://developer.mozilla.org/en-US/docs/Web/API/WindowOrWorkerGlobalScope/setInterval

## Project 3
This project incorporated using html sliders to change the value of CSS elements.
I learned how to convert the input values from the slider into the CSS variables.

CSS Variables
https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_variables

CSS Variables are created by pre-fixing -- to the name of the variable.

--base: yellow;
--blur: 10px:
--spacing: 10px

Applying the variables to elements you must wrap them in var(--customVariable)

    img{
      padding: var(--spacing);
      background: var(--base);
      filter: blur(var(--blur));
    }

I also learned about :root a CSS pseudo-class, which represents the root of the document.
https://developer.mozilla.org/en-US/docs/Web/CSS/:root
:root {
    --base: yellow;
    --blur: 10px:
    --spacing: 10px
}

## Project 4
This project focused on practicing the JavaScript array methods
 .filter() .map() .sort() .reduce()
While utilizing ES6 Syntax

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter
Array.filter() creates a new array with elements that meet the test criteria provided by the function.

let words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];
const result = words.filter(word => word.length > 6);
// expected output: ["exuberant", "destruction", "present"]


https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map
Array.map() creates a new array applying the applying the function call on each element.

let array = [1, 4, 9, 16];
const map = array.map(x => x * 2);
// expected output: [2, 8, 18, 32]

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort
Array.sort() sorts the element of an array in place and returns it.

var array1 = [1, 30, 4, 21];
array1.sort((a,b) => a -b);
// Expected Output [1, 4, 21, 30]


https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reduce
Array.reduce() Runs a function provided on each element of the array making a single value.

## Project 5
https://www.w3schools.com/css/css3_flexbox.asp
Mostly FlexBox with CSS

Learned to use Flex: 1 / Flex: 5

You can display: flex; on both the parent container and the child element to create dynamic layouts

## Project 6
This section was cool. I learned about API Calls and Regular Expressions

This is a function to add commas to numbers 1,000 520,652 etc...
function numComma(x) {
  return x.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ',');
}

https://www.regular-expressions.info/
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions
Regular Expressions are very powerfull and handy especially when masterd. I learned about:
-g global
-i case insensitive.

Also creating regex variables so you can store the expression in a variable to easily use it.
const regex = new RegExp(wordToMatch, 'gi');

https://www.taniarascia.com/how-to-connect-to-an-api-with-javascript/
https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Introduction

API calls using  fetch and then. You get an endpoint usually a json list of objects/items
const endpoint = 'https://gist.githubusercontent.com/Miserlou/c5cd8364bf9b2420bb29/raw/2bf258763cdddd704f8ffd3ea9a3e81d25e2c6f6/cities.json';
const cities = [];

https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/then
fetch(endpoint)
.then(blob => blob.json())
.then(data => cities.push(...data))



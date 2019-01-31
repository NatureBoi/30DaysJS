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
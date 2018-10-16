### Problem Set 2

#### 1. DOM Manipulation

- a. Write a function that if entered into the terminal, will convert all text on a Wikipedia page into Pig Latin (look up the rules of Pig Latin).

- b. Write an event listener that if entered into the terminal, will give the user the ability to delete any DOM element on the page simply by clicking it.

- c. Write an event listener that if entered into the terminal, will, on click, convert any `p` tag on the page into a text input field with its value equal to that of the contents of the `p` tag. These input fields should be accompanied by a submit button that when clicked, will switch the text input field back into a `p` tag, the contents of which should be equal to what was typed into the text input field.

Basically, you are making every `p` tag editable.

- d. Write an event listener that if entered into the terminal, will, when clicking any word on a page, look up the definition of that word and report that definition in an alert. If no definition is found, the alert should report this. You can use any dictionary API, but here's an easy one:

https://googledictionaryapi.eu-gb.mybluemix.net/


- e. Write a function that finds all the text on any webpage page and returns an array of objects containing both the sentence itself, as well as the DOM element it was within. You need only find full sentences (those ending in periods).

- f. Take the return value from the above function and the function you wrote for **exercise c from the Objects section in `problem-set-1`** and use it to analyze the text on the page. The `word_locations` data should also include the DOM element where that word was found.



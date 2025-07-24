Day 03 / Character Counter

What is referred to as characters?
Oh! Not those masked figures from your horror novels or movies.
In language and writing, characters are individual letters, numbers, punctuation marks, or symbols.

In computing, a character is a single unit of text—a letter, digit, symbol, or even a control code, each with a unique code point (usually in Unicode).

What is a Character Counter?
A character counter helps users see how many characters they’ve typed into a text area.
For example, when filling out an "About Me" form with a character limit, the counter tells you how many characters you've used or have left.

Step-by-Step Explanation
1. HTML: Set Up the Text Area
You'll need:

A <textarea> where users type their text.

A <div> or <p> tag to display the character count.

2. JavaScript: Add the Counter Logic
Here’s what to do:

First, declare two variables:

One for the text area.

One for the counter display.

javascript

const text = document.getElementById("text");
const counter = document.getElementById("counter");
Then, use addEventListener to listen for user input:


text.addEventListener("input", () => {
  counter.textContent = text.value.length;
});
Let's break it down:
addEventListener("input", ...): This tells the browser to do something whenever the user types (input) in the text area.

() => {...}: This is a short form of writing a function, also called an arrow function.

You could also write it like:


text.addEventListener("input", function() {
  // your code
});
Inside the function:

counter.textContent = text.value.length;
counter: The variable holding the display element.

textContent: A property used to change or get the text inside an HTML tag.

text.value: The actual text typed in the textarea.

.length: Gives the number of characters typed.

That’s it for Day 03!
DON'T JUST READ!!
try it out.
Test it once, twice, three times. Even more. until you truly understand and remember it.

Practice makes mastery.

See you on Day 4! 

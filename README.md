# Learning-log
## 2025/09/12 Morning
Topic: DOM Manipulation and Events with The Odin Project

- Types of web page manipulation possible with JavaScript
- Realization: Previously, I had an item that I couldn't click on in Python, so I automated the process using JavaScript web page manipulation code, and now I've created something a little familiar.
- Next up: Tonight, I'll continue studying Revisiting Rock Paper Scissors.

## 2025/09/16 Morning
Topic: Event Listeners and DOM Updates with JavaScript

Clarified the difference between event listeners and event handlers.

Understood why textContent is safer and clearer than innerHTML for adding plain text.

Realized that combining DOM manipulation with events is the foundation of making interactive web pages.

Next up: Tonight, I’ll continue with Rock Paper Scissors, this time adding event-driven interactions instead of relying only on prompts.


## 2025/09/16 Evening

What I Did Today

Learning Topic: DOM Manipulation and Event Handling

Based on the "shopping-list.html" starter file, I prepared a state with minimal CSS, labels, input fields, a button, and an empty <ul>.

Stored references to <ul>, <input>, and <button> in variables.

Created a function called handleClick that executes when the button is clicked.

Retrieved the value of the input element and saved it in a variable.

Empty the input field.

Created three new elements: <li>, <span>, and <button>.

Displayed the input value in the <span> and added a delete label to the <button>.

Added a <span> and <button> to the <li> and appended them to the <ul>.

What I Learned

The importance of using document.querySelector to retrieve HTML elements and store them in variables.

createElement and appendChild How to dynamically add elements using CSS.

Using an event listener to execute a function when a button is clicked

Creating a new element within a function allows you to generate a separate <li> element for each click.

Next steps

Add a click event to the added delete button to delete the list item.

Practice applying dynamic styles using CSS classes.


## 2025/09/16 Morning

# Shopping List DOM Practice

**Topic:** Event Listeners and DOM Updates

**What I Did:**
- Prepared starter HTML with minimal CSS, input, button, and empty list.
- Stored references to `<ul>`, `<input>`, and `<button>` in variables.
- Created `handleClick` function for button clicks.
- Retrieved input value and cleared input field.
- Created `<li>`, `<span>`, `<button>` elements.
- Set `<span>` textContent to input value and `<button>` textContent to "delete".
- Appended `<span>` and `<button>` to `<li>`.
- Added `<li>` to `<ul>`.
- Attached click event to delete button to remove the `<li>`.
- Focused input field after adding an item.

**What I Learned:**
- How to dynamically create and append elements using JS.
- Difference between event listeners and handlers.
- Using closures to maintain individual item behavior.

## 2025/09/17 Night

# What I worked on today
- Continuing the Rock Paper Scissors project
- Removed the "logic to play exactly 5 rounds (for loop)" from the `playGame()` function
- Prepared for future UI implementation by making the game progression more flexible.

# What I learned/observed
- When manipulating the DOM with JavaScript, you can add nodes to the element tree using appendChild.
- I understood how adding a child element and then appending it to the parent element reflects the changes in the browser.
- `textContent` is used to insert text into an element and does not affect the tag itself.
- When using Git, it's important to keep in mind the following sequence: "Initialize the repository" → "Add files" → "Commit" → "Push to remote."

# Next steps
- Proceeding with the Rock Paper Scissors UI implementation
- Using HTML and CSS to create buttons that can be clicked to advance the game.
- Creating a branch on GitHub (`rps-ui`) and proceeding with UI development.


## 2025/09/18 Morning
# Top Rock-Paper-Scissors
Overview

This morning, I worked on the Top Rock-Paper-Scissors project. The focus was on JavaScript DOM manipulation and event handling to prepare for an interactive UI version of the game.

What I Did

Set up HTML and references

Prepared the starter HTML with buttons for "Rock", "Paper", and "Scissors".

Stored references to these buttons in JavaScript variables for easier access.

Created event listeners for each button

Defined a function to handle a click on each button.

Each click updates a variable representing the player's choice.

Integrated player choice with existing game logic

Prepared the system to pass the player's selection into the existing playRound function.

The function already exists and calculates round results based on player and computer choices.

Kept console logging for debugging

Console outputs were used to verify that player choices and round results are correct.

Key Learnings

How to attach event listeners to buttons and capture user interaction.

Connecting UI elements to game logic without using prompts.

Understanding asynchronous event handling: the function waits for user clicks rather than executing sequentially.

Reinforcing the separation between data (player choice) and logic (round evaluation).
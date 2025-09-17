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
DOM Manipulation and Events — The Odin Project

Overview

Today, I practiced JavaScript DOM manipulation and event handling using the "shopping-list.html" starter file from The Odin Project. The focus was on dynamically creating elements, attaching event listeners, and manipulating the DOM to make an interactive shopping list.

What I Did

Set up references to HTML elements

Stored references to the <ul>, <input>, and <button> elements in variables for easier access.

Created a function to handle button clicks

Defined a function called handleClick to execute whenever the "Add" button is clicked.

Retrieve input value and reset input

Stored the value from the input field in a variable.

Cleared the input field after storing the value.

Created new elements dynamically

Created <li>, <span>, and <button> elements.

Added the <span> and <button> as children of the new <li>.

Set content for span and button

Set the <span> text to the value entered by the user.

Set the button text to "delete".

Append new <li> to the list

Added the <li> as a child of the <ul> to display it on the page.

Attach event listener to the delete button

Clicking the delete button removes the corresponding <li> element from the list.

Refocus input field

Used the .focus() method to move the cursor back to the input field, making it ready for the next item.

Key Learnings

How to use document.querySelector to select HTML elements.

The difference between textContent and innerHTML for safely inserting text.

Dynamically creating elements with createElement and appending them with appendChild.

Attaching event listeners to elements for interactive functionality.

Using .focus() to improve user experience in forms.

Next Steps

Continue integrating DOM manipulation with event-driven interactions in other projects.

Explore additional CSS styling for dynamically added elements.

Experiment with other input types and validation for user entries.
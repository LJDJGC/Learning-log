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

## 2025/09/18 Evening
Topic: Rock-Paper-Scissors Web Game (DOM Output Edition)
1. Objectives

Create a "Rock-Paper-Scissors" game in the browser

Select the player's move with button presses

The computer's move is random

Display the result and score on the screen

The first player to score 5 points wins the game

2. Learning Content and Progress
a) Initial Implementation

Consistently check the result and score with console.log()

Randomly select the computer's move with getComputerChoice()

Input from the button with getHumanChoice()

Determine the winner of a round with playRound(humanChoice, computerChoice)

b) Modify for DOM Output

Add a <div id="result"></div> to the HTML to display the results

Replace console.log() with resultDiv.textContent = ...

First, check by displaying only the results of the most recent round

Take small steps and change the display destination from console → Practice "changing to DOM"

c) Score Management

Define humanScore and computerScore as global variables

Update the score after determining the winner in playRound()

Call playGame() at the end of the round to determine the winner when the player reaches 5 points

3. Learning Discoveries and Challenges

Calling playGame() at the end of playRound() overwrites the round results

Displaying progress and the final winner requires careful consideration of div usage and display methods

If outputting as a history, it is more appropriate to use appendChild

Currently, we are testing the "overwriting display of the most recent round + score" option

4. Next Challenge

Organize a method for simultaneously displaying round results and scores

Consider using separate divs for the win/loss message and score, or displaying both in a single div

Add a mechanism to stop the game when a final winner is announced

5. Review of Learning

Event Listeners and DOM Learn how to coordinate outputs

Understand the importance of functional separation of responsibilities (deciding whether a game is won or lost, updating the score, and determining the winner)

Realize the effectiveness of iteratively checking and correcting in small increments

## 2025/09/19 Morning
Topic: Rock Paper Scissors UI (DOM Manipulation and Event Listeners)

- I started implementing a button-based rock-paper-scissors game using a combination of HTML and JavaScript.
- I encountered an error where `querySelector` returned `null`. I realized the cause was the timing of script execution and the order of HTML elements.
- Solutions:
- Move `<script>` to the end of the HTML.
- Or use `<script defer>` to execute it after the DOM is constructed.
- I also discovered a spelling mistake: `id="conputerResult"`, which needed to be changed to `computerResult`.
- I learned that small spelling errors and script loading order can quickly lead to "element not found" bugs.

Next, I'll test the UI again after making the corrections to ensure it displays correctly.

## 2025/09/24 Morning  
Topic: Rock Paper Scissors UI – Git, Branch Merge, GitHub Pages Deployment  

- Implemented **UI for Rock-Paper-Scissors** game (start button, score tracking, reset).
- Fixed issue where final result message disappeared too quickly → added `setTimeout` before reset.
- Controlled game flow with **disable/enable buttons** until "Start Game" is pressed.
- Learned how to **merge feature branch (`rps-ui`) into `main`** using `git checkout main` + `git merge rps-ui`.
- Cleaned up understanding of **committed vs. uncommitted changes** (merge showed "Already up to date" because edits weren’t committed yet).
- Successfully **pushed changes to GitHub**.
- Published project on **GitHub Pages** and confirmed live URL:  
  👉 [Live Demo](https://ljdjgc.github.io/top_rock-paper-scissors/)

Next up: Update README with project description and live preview link.

## 2025/09/24 Evening 

# Etch-a-Sketch Project

- Created a repository on GitHub and confirmed the process of connecting it to a local repository.
- Learned the basic operations of `git init` → `git remote add origin` → `git branch -M main` → `git push`.
- Created a README and completed the first commit and push.

- Reviewed the project assignment instructions.
- The goal was to generate a 16x16 grid using JavaScript.
- Dynamically added elements using a loop instead of directly arranging divs in HTML.
- Understood how easily a square can be created using CSS Grid and `aspect-ratio`.

- Organized implementation tips.
- Created cells using `document.createElement` and `appendChild`.
- Added cells efficiently using `DocumentFragment`.
- Confirmed the idea of ​​coloring cells with the `mouseover` event.

## Next Steps
- Actually created a 16x16 grid. Generate cells and display them in the browser.
- Implement a mechanism for changing cell color on hover and click.
- As a finishing touch, make the number of cells freely adjustable.

## 2025/09/25 Morning

Topic: Creating a 16x16 grid div with JavaScript and displaying it with Flexbox

- Preparing a `.container` div in HTML
- Creating a 16x16 div in `script.js` using `document.createElement` and `appendChild`
- An error occurred with the initial JS code:
- `count` in `console.log(myContainer, count);` was undefined → Changed to `i`
- Corrected `document.body.appendChild(...)` to `myContainer.appendChild(...)`
- Checking the display with CSS:
- Setting `display: flex; flex-wrap: wrap; width: 500px;` to `.container`
- Set `flex: 0 0 calc(100% / 16);` and `aspect-ratio: 1 / 1;` to the `.container div`.
- 0 height issue:
- This can be resolved by removing the `height` from the `.container` or by setting the cell to `height: calc(500px / 16);`.
- Set the background color `lightgray` to ensure the generated div looks correct.
- Currently, the 16x16 square grid is ready to be displayed using a combination of JS and CSS.

Next step:
- Add hover color behavior similar to Etch-a-Sketch.

## 2025/09/25 Night
Topic: 16x16 Grid Generation and Hover Effects with Flexbox

Lessons

Used JavaScript to dynamically generate 16x16 div elements without writing HTML.

Using Flexbox's flex-wrap and flex: 0 0 calc(100% / 16) to create a layout with 16 wrapped squares.

Confirmed that gaps and borders would cause the squares to collapse, and achieved a stable display with gap: 0.

Added mouseover event listeners to each generated div and applied a class to create a "trail" effect that changes the background color.

I learned

Executing document.createElement("div") once outside of a loop reuses the same element, resulting in incorrect generation of 256 divs.

Instead of writing classes directly in the HTML, dynamically using classList.add() in JavaScript is necessary for the "leave a trail" mechanism.

Even with Flexbox, care must be taken when handling gaps. You can include them in the calculation formula if necessary.

Next Steps

Combine mousedown / mouseup to allow drawing by dragging the mouse.

Expand the color from a fixed (black) to random or a gradual change in density.

Create a reset button to refresh the entire grid.
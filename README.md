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

## 2025/09/28 Night

Topic: Creating a Pixel Drawing Grid Using CSS Grid
Learned Content

I created a 16x16 div element in JavaScript and tested a mechanism for changing its color with mouse operation.

I experimented with using flexbox on the .container in CSS to evenly distribute the cells.

I then switched to a grid layout and improved the implementation.

Key Points

The cell arrangement is specified on the container side (e.g., grid-template-columns).

The cell's appearance (background color, aspect ratio) is specified in the CSS for the child element.

flex-wrap is not required for grid.

Next Steps

Consider changing the cell color from fixed black to a random or selected color.

I will try extending it to more pen-like behavior, such as "draw only while clicked."

Make the grid size variable (e.g. 16x16 → 32x32).

## 2025/09/29 Morning 
In today's lesson, we worked through the steps of combining JavaScript and CSS to create an **interactive grid sketchpad**. The basic process was to first create a `.container` in HTML and then create a 16x16 div in JavaScript to create a grid. We maintained the square shape by using `aspect-ratio: 1/1` and managed the color by specifying `background-color` in CSS.

Looking back internally, at first, we realized that all we could see was black lines. We stopped and thoroughly checked the HTML structure, CSS class application, JavaScript variable references, etc. In particular, we noticed that we had incorrectly handled the i and square variables in the for loop, and that a CSS priority issue (a conflict between background and background-color) was preventing the colors from being reflected. We corrected these issues step by step.

By adding !important to the CSS .colored class and confirming that the class was actually added in the browser's developer tools, we were able to complete the color change function on mouseover. In this way, we were able to create a "pen"-like feature that turns black when you trace it with the mouse.

As a next step, we considered adding a button to the top of the screen that would delete the existing grid and generate a new grid with the same total area based on the new grid size entered by the user. Here, we reorganized the flow: obtaining input using prompt, limiting the maximum value (100), clearing using innerHTML = "", dynamically changing grid-template-columns, and again generating divs and attaching events. This resulted in a design that would allow a new sketchpad to be generated without changing the area, even for a 64x64 grid.

Through today's learning, I reaffirmed the importance of not simply writing code, but thoroughly verifying and understanding small elements such as CSS priority, JavaScript variable scope, DOM manipulation, and event firing timing. I found the process of identifying and checking each issue one by one to be extremely effective.

Next time, I plan to implement a button that generates grids based on user input, creating a more flexible and interactive sketchpad.

Today's Achievements

Completed 16x16 grid generation and hover-color change functionality

Understood CSS precedence issues and applied the .colored class

Now I can check class assignments in the developer tools

Refine the design of the dynamically resizable grid generation for next time

## 2025/09/29 Night
Topic: JavaScript Grid Generation and Hover Event Verification
1. Today's Lessons

Creating a system that changes the color of grid cells when hovered using HTML/CSS/JS

Displaying an initial 16x16 grid and allowing it to be resized with a reset button

Creating a div within a for loop and attaching a mouseover event

On reset, deleting existing cells and creating new ones with container.innerHTML = ""

Analyzing the cause of hover issues

Checking whether event listeners are attached correctly

Div size issues when CSS aspect-ratio doesn't work

Tips for isolating the problem:

Check whether events are being fired with console.log

Check the div size and class attachment in DevTools

If aspect-ratio doesn't work, test with a fixed height

2. Today's Lessons Learned and Awareness

If hover isn't working, first check whether an event is attached and whether the div "Does the size of this exist?" is questionable.

Operations on innerHTML must be performed outside the loop, or the grid will disappear.

The initial grid and post-reset grid generation processes are easier to manage if they are created as functions.

## 2025/09/30 Morning

This project uses JavaScript and CSS to create a 16x16 square grid, and creates a sketchpad that changes the mass color according to the user's mouse interaction.

Today's study content

Grid creation

Using JavaScript's document.createElement, create a 16x16 div element and place it inside the .container

Grid viewing using Flexbox

CSS display: flex; flex-wrap: wrap; realizes a grid that wraps side by side

Adjusting the square size

The width and height of each square are calculated and set using JS.

Color change during hovering

Initially, set the fixed color purple in CSS

Next, we will consider how to randomly generate RGB values ​​in JavaScript and change the color for each hover.

Issues and prospects for the next episode

To implement the effect of darkening by 10% in stages, we consider a design that maintains the state of each square with dataset.

Confirmed that random colors and gradual darkening cannot be achieved for each interaction with CSS alone

File configuration

index.html … HTML for grid display

style.css … Flexbox Grid, Mass Initial Style

script.js … Grid generation, color change processing by hover event

How to use

Open index.html in your browser

Create a grid of any size with the Reset button

Hovering the mass with the mouse changes color

## 2025/09/30 Evening
What I did today

Improved the square interaction function in the Etch-a-Sketch project

Implemented a system where each square changes to a random color when hovered, then gradually darkens after 10 hovers, finally reaching black.

Learned how to save the state of each square (base color and hover count) using dataset.

Introduced logic to generate a random color only the first time using if (!square.dataset.base) and darken the color based on the saved base color thereafter.

I confirmed that confusion between dataset.hover and dataset.hovers was the cause of the bug and understood that it needed to be fixed.

What I learned

Dataset makes it easy to store state in DOM elements.

The importance of separating "first-time processing" from "repeated processing" in event handlers.

To "darken the color," calculating it based on RGB values ​​rather than lowering opacity works better than "darkening the color"

What I'll do next

Modify dataset.hovers to use it correctly.

First hover Sometimes I decide whether to "color it as is" or "darken it by 10%."

Code organization (removing unnecessary console.log and standardizing variable names)

## 2025/10/01
Learned

Learned the basics of JavaScript objects

How to create objects, add and reference properties

Manage data for DOM elements using datasets

Dynamically create a 16x16 Flexbox grid using HTML/CSS/JS

Create divs using the createGrid() function

Place the grid within a .container

Arrange elements in a grid using flex-wrap in CSS

Set an event to change the color of each div on mouseover

Each div is initially a random color, then gradually darkens by 10% with each click or mouse action

Create a new grid size with the "Reset" button

Maximum input size is 100x100

Check hover counts in console.log for debugging

Today's Takeaways

Using objects makes it easy to manage information such as hover counts and base color for each div

Direct manipulation of the DOM and datasets You can maintain state by combining these.

Creating a grid with Flexbox makes it easy to arrange elements in rows and columns without using CSS Grid.

Combining clicks and mouseovers allows you to create gradual, pen-like movements.

GitHub Repository Setup Notes

File Structure Example:

/project-root
index.html
style.css
script.js
README.md

Commit messages should be small and frequent.

Example: October 1, 2025, Morning: Created a 16x16 grid, with color changes and gradual darkening on mouseover.

Publishing to GitHub Pages:

index.html must be in the root directory.

Select the branch and root in Settings > Pages.

Note the public URL and add it to the README.

About Live Preview (Live View)

If you're using Visual Studio Code, the Live Server extension is useful.

After installation, right-click index.html and select Open with Live Server.

The browser will launch automatically and reload automatically when changes are made.

You can also publish to GitHub Pages and view it in your browser.
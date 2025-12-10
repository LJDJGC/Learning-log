📝 Today I Learned (TIL)
Topic: The Odin Project - Intermediate HTML and CSS (Advanced Selectors)
Today, I continued reading Shay Howe’s article on Complex Selectors as part of The Odin Project's Advanced Selectors section in the Intermediate HTML and CSS Course.

To enhance my learning, I practiced in Codepen and manually verified which elements each selector was targeting. This active output method significantly boosted my learning efficiency.

I also moved on to the Selectors Assessment from MDN. While my overall learning speed has slowed down, I feel that actively coding and performing self-checks is greatly improving my understanding. I realize that my study efficiency is still not fully maximized, so I plan to continue searching for better methods while utilizing Anki and Active Recall to ensure better knowledge retention.

📝 TIL (Today I Learned) Log - December 10, 2025
Focus Area: The Odin Project - MDN CSS Selectors Assessment
I spent time working on the CSS Selectors Assessment from The Odin Project (via MDN).

Learned/Completed Tasks
I successfully implemented basic attribute and pseudo-class selectors. However, I encountered specific challenges where my intended CSS was not behaving as expected.

Challenges & Unresolved Issues
I feel that I still have gaps in my understanding of the following specific CSS selector and property rules:

1. Multiple Class Selectors (Combinators)
I struggled with combining multiple class selectors to apply specific styles:

Goal 1: Set the background of an element with both the .alert class and the .stop class to red.

Intended Selector: .alert.stop { background-color: red; }

Goal 2: Set the background of an element with both the .alert class and the .go class to green.

Intended Selector: .alert.go { background-color: green; }

I need to confirm if I am correctly using the compound selector format (writing classes immediately next to each other, with no space) versus the descendant combinator (using a space).

2. Styling Visited Links
I was unable to successfully set the color of visited links to green.

Issue: My attempts to use a:visited { color: green; } did not change the link color after visiting the page.

Hypothesis: This may be due to browser privacy restrictions on styling the :visited pseudo-class, or a CSS specificity issue where another selector is overriding it.

3. Pseudo-elements and Combinators
I was also stuck on a multi-part styling task:

Goal: Set the first element inside a container to font-size: 150%, AND set the first line of that specific element to red.

The specific issue: I struggled with correctly targeting the first line using the ::first-line pseudo-element after selecting the first element using a pseudo-class like :first-child or :first-of-type.

Plan for Tomorrow
I recognize these are critical concepts related to specificity, pseudo-classes, and pseudo-elements. Tomorrow, I plan to thoroughly read the corresponding MDN documentation and tutorials to resolve these three specific issues. I will focus particularly on the distinction between the compound selector (.class1.class2) and the descendant selector (.class1 .class2).
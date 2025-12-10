Today I Learned (TIL)

I was working on the MDN test to change the color of visited links using a selector. I tried writing:

CSS

a:visited {
    color: green;
}
However, it didn't work (the link color didn't change). I decided to move on and check the provided solution later.

When I checked the solution, it was written exactly the same way. I suspect the issue might be related to a version change or browser security restrictions.

Next, I'm moving on to Task 4. I already started Task 4 this morning. I really hope to finish all the MDN tasks by the end of today.

📝 Note (Note on the CSS issue)
The CSS :visited pseudo-class has very strict restrictions on the style properties it can apply for privacy and security reasons.

The color property is one of those restrictions, but browsers often limit its display to a default color or a color that offers little contrast with the usual link color. Due to security restrictions, the reason a:visited { color: green; } doesn't work may be due to MDN's testing environment or browser settings.
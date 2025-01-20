# CSS Specificity Bug: Unexpected Color Inheritance

This repository demonstrates an uncommon CSS specificity issue where the expected color inheritance does not occur due to selector specificity and the order of CSS declarations.  The bug arises in some browsers due to how they calculate selector specificity, where a less specific selector can override a more specific selector if it appears later in the stylesheet.

## Bug Description
The `bug.css` file contains CSS code causing the problem.  The expected outcome is that text within paragraphs in divs with the class "container" should appear blue.  However, this is not always the case in all browsers.  The `bugSolution.css` shows how to solve the problem.
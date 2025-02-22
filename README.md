# CSS Specificity Gotcha: Rule Order and Unexpected Width

This repository demonstrates a subtle bug related to CSS specificity and the order of CSS rules.  The issue highlights a situation where the most specific selector doesn't always win due to how the CSS cascade works.

## Bug Description

The `bug.css` file contains CSS rules that demonstrate unexpected behavior due to the interaction between specificity and the order of rules. Although  `#myId .container.myClass` has the highest specificity, the result might differ from the expected 100px width, depending on the order of the rules. This is because of the way CSS processes rules in a cascading order.

## Solution

The `bugSolution.css` file provides a solution by reorganizing the CSS rules to ensure that the most specific rule always takes precedence, regardless of its position in the stylesheet.  It's best practice to place the most specific rules last to mitigate this uncommon issue. 
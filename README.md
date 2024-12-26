# Uncommon CSS Specificity Bug

This repository demonstrates an uncommon bug related to CSS selector specificity.  Despite a more specific selector existing, the expected styling is not always applied. This behavior can be inconsistent across different browsers. 

The bug arises from the complex calculation of selector specificity in CSS. This example highlights a situation where the expected behavior, based on typical understanding of specificity, does not occur.

## Reproduction Steps

1. Clone this repository.
2. Open `index.html` in your web browser.
3. Observe the rendered width of the `.item` div.  It might not be 20% as expected, due to specificity issues.

## Solution

The solution involves re-evaluating the specificity of the selectors and adjusting the CSS to ensure that the desired style is applied consistently. This could involve more specific selectors or the use of `!important` (though generally discouraged).

See `bugSolution.css` for a possible fix.
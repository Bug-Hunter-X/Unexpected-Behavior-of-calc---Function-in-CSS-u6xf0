# Unexpected Behavior of calc() Function in CSS

This repository demonstrates an uncommon bug related to the `calc()` function in CSS. The bug arises when using percentages and other units together within the `calc()` function, or when nesting `calc()` functions.  The behavior is inconsistent and can lead to unexpected layout issues.

## Bug Description

The `calc()` function in CSS is designed to perform calculations to determine property values.  However, when combining percentages with fixed units (like pixels), or when nesting `calc()` expressions, unexpected results may occur.  This often deviates from the mathematically expected outcome.

## How to Reproduce

1. Clone this repository.
2. Open `bug.css` to see the problematic code examples.
3. Observe the rendered output in a browser.  The actual width of the elements will differ from the expected width based on a straightforward mathematical interpretation of the `calc()` expressions.

## Solution

The solution is to avoid complex `calc()` expressions or to carefully consider the order of operations when using multiple units.  In some cases, rewriting the CSS using different approaches (e.g., using separate classes and adjusting margins) can resolve the problem.  Refer to `bugSolution.css` for examples of workarounds.
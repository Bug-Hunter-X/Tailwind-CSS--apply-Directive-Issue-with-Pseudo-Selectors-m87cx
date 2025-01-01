# Tailwind CSS @apply Directive Issue with Pseudo-Selectors

This repository demonstrates a bug where Tailwind CSS's `@apply` directive doesn't correctly apply styles when used with pseudo-selectors like `:hover`, `:focus`, or `:active`.

## Bug Description

The `@apply` directive, intended for applying pre-defined styles, fails to apply styles associated with pseudo-selectors. This leads to unexpected visual behavior, as the intended hover, focus, or active states are not correctly rendered.

## Solution

The solution involves applying the styles directly within the element's class list, rather than relying on the `@apply` directive for pseudo-selectors.  Directly applying the styles ensures that they are correctly linked to the respective states.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in your browser.  Observe that the hover effect does not work as expected.
3. Then open `bugSolution.html` to see the corrected implementation.

## Technologies Used

* HTML
* CSS
* Tailwind CSS
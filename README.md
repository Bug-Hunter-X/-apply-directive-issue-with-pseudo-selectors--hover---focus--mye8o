# Tailwind CSS @apply Directive Issue with Pseudo-selectors

This repository demonstrates a bug where Tailwind CSS's `@apply` directive doesn't correctly apply styles when used with pseudo-selectors such as `:hover` or `:focus`.  The issue is that the styles defined within the `@apply` directive for these pseudo-selectors are not applied to the elements as expected.

## Bug Description

When using the `@apply` directive with a class containing a pseudo-selector (e.g., `hover:bg-blue-700`), the styles associated with that pseudo-selector are not applied when the corresponding condition (hover, focus, etc.) is met.

## Steps to Reproduce

1. Clone this repository.
2. Open `index.html` in a web browser.
3. Observe that the button's background color doesn't change on hover, despite the CSS rules appearing correct.

## Solution

The solution is to apply the pseudo-selector styles directly to the element, instead of using the `@apply` directive with pseudo-selectors.
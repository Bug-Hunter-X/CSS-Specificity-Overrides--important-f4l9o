# CSS Specificity Overrides !important

This repository demonstrates an uncommon CSS bug related to specificity overriding the `!important` declaration.  The bug highlights a situation where a more specific selector's style rules take precedence, even over those using `!important`.

## Bug Description

A common assumption is that `!important` always overrides all other styles.  However, this is only true unless a more specific selector is used.  This example shows how a higher specificity selector overrides an `!important` declaration.

## How to Reproduce

1. Open `bug.css`.
2. Inspect the rendered styles of the `.child` element within the `.parent` element.  You'll observe the color is green, despite the `!important` declaration.
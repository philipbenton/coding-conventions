CSS
===

This document outlines the conventions we use at [It's Good Practice](http://www.itsgoodpractice.com) for writing CSS code. It should be strictly applied, and any exception to the rule be discussed first.

## Table of Contents

1. General Principles
2. Whitespace
3. Comments
4. Format
5. SASS/SCSS
6. Practice Example
7. Derived From

## 1. General Principles

## 2.

## Comments

Well commented code is extremely important. Take time to describe components, how they work, their limitations, and the way they are constructed. Don't leave others in the team guessing as to the purpose of uncommon or non-obvious code, what may seem or feel transparent and self explanatory to you may not be to another developer.

Comment style should be simple and consistent within a single code base.

* Place comments on a new line above their subject.
* Keep line-length to 80 characters.
* Make liberal use of comments to break CSS code into discrete sections.
* Use "sentence case" comments and consistent text indentation.

Tip: configure your editor to provide you with shortcuts to output agreed-upon comment patterns.

Example:

```css
/* =======================================================================
   Section comment block
   ======================================================================= */

/* Sub-section comment block
   ======================================================================= */

/**
 * Short description using Doxygen-style comment format
 *
 * The first sentence of the long description starts here and continues on this
 * line for a while finally concluding here at the end of this paragraph.
 *
 * The long description is ideal for more detailed explanations and
 * documentation. It can include example HTML, URLs, or any other information
 * that is deemed necessary or useful.
 *
 * @tag This is a tag named 'tag'
 *
 * TODO: This is a todo statement that describes an atomic task to be completed
 *   at a later date. It wraps after 80 characters and following lines are
 *   indented by 2 spaces.
 */

/* Basic comment */
```
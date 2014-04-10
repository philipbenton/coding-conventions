CSS
===

This document outlines the conventions we use at [It's Good Practice](http://www.itsgoodpractice.com) for writing CSS code. It should be strictly applied, and any exception to the rule be discussed first.

## Table of Contents

1. General Principles
2. Whitespace
3. [Comments](#comments)
  * [Selectors](#selectors)
  * Tags
  * Todo's
4. Format
5. [SASS/SCSS](#sass-scss)
6. Minification
7. Practice Example
8. Derived From

## 1. General Principles

## 2.

<a name="comments"></a>
## Comments

Well commented code is extremely important. Take time to describe components, how they work, their limitations, and the way they are constructed. Don't leave others in the team guessing as to the purpose of uncommon or non-obvious code, what may seem or feel transparent and self explanatory to you may not be to another developer.

Comment style should be simple and consistent within a single code base.

* Place comments on a new line above their subject.
* Keep line-length to 80 characters.
* Make liberal use of comments to break CSS code into discrete sections.
* Use "sentence case" comments and consistent text indentation.

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
 */

/* Basic comment */
```

<a name="selectors"></a>
### Selectors

Selectors should never be qualified; we should never write for example `ul.nav{}` rather just `.nav`. Qualifying selectors decreases selector performance, inhibits the potential for reusing a class on a different type of element and it increases the selector's specificity.

However, where possible, it is wise to communicate to the next developer(s) where you intend a class to be used. As an example `.product-page` sounds as though it would be used on a high-level container, perhaps the `html` or `body` element, but with `.product-page` alone it is impossible to tell.

By commenting out the leading type selector we can communicate where we wish to have this class applied:

```css
/*html*/.product-page {}
```

or, where more than one potential type selector is applicable:

```css
/*html, body*/.product-page {}
```

It is now clear where we intend to use this class without any of the drawbacks.

<a name="sass-scss"></a>
## SASS/SCSS

**Note:**

_The principles outlined in this document are adhered to on the few occasions we're **NOT** using SASS/SCSS to pre-compile our CSS code._

However, when writing code in SASS/SCSS many of the principles outlined in this document will cross over and be similar, view the [SCSS document here](https://github.com/philipbenton/coding-conventions/blob/master/SCSS.md).
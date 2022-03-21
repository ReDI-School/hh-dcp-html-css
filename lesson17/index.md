---
title: Lesson 17 - Cascade, Specificity and Inheritance
nav_order: 17
---

# Cascade, Specificity and Inheritance

In this class, we want to improve our understanding of how CSS applies the styles we write on the HTML elements.

Students should be able to understand situations like: what happens when there are conflicting rules, and what happens if multiple selectors are attempting to add a style to an element.

Note: Teachers are not limited to the examples shown in this note.

## Class Agenda

- Precedence
- Specificity
- Inheritance
- !important

# Introduction

The word "Cascading" in Cascading Style Sheets is a key concept to understand. As your webpage styles increases, you may have a situation where a particular CSS rule you just wrote is not applying to the element because another rule is taking Precedence, or because of a specificity case. We explore these concepts below.

# Precedence

When multiple CSS rules are used on an element at the same specificity level, CSS needs to decide which rule to apply to the element. When this situation happens, the rule that comes last in the source code will be used. Examples:

```css
/* Example 1 */
/* If you have multiple places in your stylesheet(s) where the background is
defined for the h1 tag like below, the pink background will be applied
because it comes last. */

h1 {
  background: red;
}

h1 {
  background: pink;
}
```

```css
/* Example 2 */
/* If you have an h1 with two classes like this:
<h1 class="heading top-heading">Heading</h1>, and you applied the same
css rule with the different classes as shown below, the last one that 
comes last in the source code will be used (i.e padding: 0)
*/
.heading {
  padding: 50px;
}

.top-heading {
  padding: 0;
}
```

# Specificity

Specificity is how CSS decides which rule to apply when there are multiple rules targeting an element using different selectors or source location (e.g inline style, element selector, class selector, id selector).

## Inline Styles

If you use the HTML **style** attribute to apply styles to an element, that style will override any other styles defined in a `<style>` tag or a stylesheet.

Example:

Consider a heading like this:

```html
<h1 class="heading" id="main-h1" style="color: red">Heading</h1>
```

```css
/*
 The color rule (red) defined in the style attribute will always win over
 other color values defined using CSS selectors
*/
.heading {
  color: pink;
}

#main-h1 {
  color: blue;
}
```

## Selector Specificity

Different types of selectors have different specificities. For example, an ID selector has a higher specificity than a Class selector, while a Class selector has higher specificity than an Element selector. In this section, we want to show (with examples) how different selector rules are ranked and which ones win over the others.

```css
/* Consider an example with a heading like this
  <h1 class="heading" id="main-h1">Heading</h1>,
  which color will be applied on the page?
*/
.heading {
  color: pink;
}

#main-h1 {
  color: blue;
}
```

# Inheritance

Inheritance is another crucial part of CSS Cascade. Inheritance is how some CSS rules, which are set on parent elements, are inherited by their child elements. In this section, we want to show examples where a property value (e.g color, font-family) is inherited by an element.

Example:

```html
<section>
  <p>This is the first paragraph in the section</p>
  <p class="note">
    This is another paragraph with <span>a span element</span> inside it
  </p>
</section>
```

```css
/* the two paragraphs inherits sans-serif font-family,
 but only the first one applies it, because the second paragraph
 has a font-family set on it. The span inherits cursive font from
 the second paragraph
 */
section {
  font-family: sans-serif;
}

.note {
  font-family: cursive;
}
```

# !important

This is a special declaration in CSS that you can use to overrule all the specificity or inheritance logic explained above. When you apply `!important` to a rule, it becomes the most specific one and overrides the normal rules of the cascade. It also overrides inline styles in the markup.

It is useful to know that `!important` exists, however, you are strongly advised not to use it unless if you absolutely need to.

# Extra Exercise

- Show how to see overridden rules using the Dev Tools. [Example](https://developer.chrome.com/docs/devtools/css/overrides/)

# Glossary & Terminology

- `Inheritance` is a process of receiving values of properties by a child element from its parent element.
- `Specificity` determines which CSS rule is applied by the browsers.

# Homework

- Look in your project and review how specific your CSS selectors are. See if you can find places you could be using lower specificity while still achieving your styling.
- In [Checkpoint 17](https://github.com/ReDI-School/nrw-html-and-css/tree/checkpoint17), we added comments to our CSS file regarding inheritance and specificity. Take a look at it, and try to find other similar places in your code and label them.

# Resources

- [Calculating CSS Specificity Value](https://css-tricks.com/specifics-on-css-specificity/#calculating-css-specificity-value)
- [MDN Cascade and Inheritance Page](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Cascade_and_inheritance)
- [MDN Specificity](https://developer.mozilla.org/en-US/docs/Web/CSS/Specificity)
- [Precedence in CSS](https://css-tricks.com/precedence-css-order-css-matters/)

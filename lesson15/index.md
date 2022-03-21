---
title: Lesson 15 - CSS Positioning
nav_order: 15
---

# CSS Positioning

## Class Agenda

1. Introduction to Positioning
2. Static Positioning
3. Relative Positioning
4. Absolute Positioning
5. Z-Index
6. Fixed Positioning
7. Sticky Positioning

# 1. Introduction to Positioning

The positioning of elements can be controlled via the CSS `position` rule. It allows you to take elements out of their normal flow. This section briefly introduces CSS Positioning and available values. This section also covers use cases for the use of different CSS Positioning values.

ETA: 5-10min

# 2. Static Positioning

This is the default positioning which HTML elements are using.

ETA: 5min

# 3. Relative Positioning

Relative positioning is a one which takes an element out of its normal flow and places it relative to its normal flow. To do this relative placement one needs to use the following CSS rules: `top`, `right`, `bottom`, `left`. This section covers this topic with more practical examples.

ETA: 15min

# 4. Absolute Positioning

Absolute positioning places elements with respect to their parent or ancestor containers. It is used to create more complex layouts and features. Absolute positioning is a very special one because it can introduce different behaviour based on the [positioning context](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning#positioning_contexts) of the element on which we apply this position type. This positioning type requires a careful explanation and analysis which would be done in class, which covers following points:

- What is absolute positioning?
- Where is it used?
- How is the absolute positioning determined?
- What are the positioning contexts?

ETA: 40min

# 5. Z-Index

An important aspect to CSS positioning is the concept of overlapping. We need to answer the question of would would happen when to elements overlap each other because of the special positioning? This section covers the CSS `z-index` rule.

ETA: 10min

# 6. Fixed Positioning

Fixed positioning fixes an element relative to the visible viewport. This section teaches this in details and shows practical examples of how we can use fixed positioning to create fixed navigation bars, as can be seen in our [Portfolio Project - Checkpoint15](https://github.com/ReDI-School/nrw-html-and-css/blob/checkpoint15/checkpoint/css/main.css#L110)

ETA: 20min

# 7. Sticky Positioning

This positioning type is a combination between relative positioning and fixed positioning. We cover it in details during the class. Moreover, we would also cover the [differences](https://dev.to/suryawiguna/css-position-fixed-vs-sticky-5232#:~:text=What's%20the%20difference%3F,offset%2C%20like%20top%3A%2010px%20.) between fixed and sticky positioning with practical examples

ETA: 10min

# Glossary & Terminology

- `Positioning` - The characteristic of elements, which defines where exactly on the webpage they are placed. Whether that is with a normal flow or taken out of the normal flow.
- `Z-Index` - The `z-index` CSS property sets the z-order (i.e. z-axis placement) of a positioned element and its descendant items. Overlapping elements with a larger z-index cover those with a smaller one. More on this can be seen [here](https://developer.mozilla.org/en-US/docs/Web/CSS/z-index)

---

# Homework

Go over checkpoint 15 and try to apply the new styles in it into your personal portfolio projects. The main aim here should be to make your navigation bar fixed. Below you can find the links to:

- [Portfolio Project - Checkpoint 15](https://github.com/ReDI-School/nrw-html-and-css/tree/checkpoint15/checkpoint)
- [What has changed between Checkpoint 15 and Checkpoint 13?](https://github.com/ReDI-School/nrw-html-and-css/compare/checkpoint13...checkpoint15). Use this link to see the differences between two checkpoints. The left panel shows the things which are removed from Checkpoint 13, whereas the right side shows the things which are added with Checkpoint 15.

Make sure to ask questions!

> There is no checkpoint 14. The previous checkpoint is checkpoint 13 because class 14 did not introduce more code to our portfolio project.

# Resources

- [Example of fixed navigation bar in the Portfolio Project - Checkpoint15](https://github.com/ReDI-School/nrw-html-and-css/blob/checkpoint15/checkpoint/css/main.css#L110)
- [Difference between fixed and sticky positioning?](https://dev.to/suryawiguna/css-position-fixed-vs-sticky-5232#:~:text=What's%20the%20difference%3F,offset%2C%20like%20top%3A%2010px%20.)
- [MDN CSS Positioning](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning)
- [Positioning context](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning#positioning_contexts)
- [W3S CSS Positioning](https://www.w3schools.com/css/css_positioning.asp)

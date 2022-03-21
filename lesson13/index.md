---
title: Lesson 13 - CSS Layout 2 - Flexbox
nav_order: 13
---

## Class Agenda

1. Introduction to Flexbox
1. The Flex model

## 1. Introduction to Flexbox

Flexbox is a comparatively newer way to layout elements on the page without the limits and frustration of Floats like:

- You have to clear Floats (when the containing element collapses).
- Sometimes have to change the order of your HTML to achieve a Floats design.

Flexbox layout makes it easier to design flexible responsive layout structure (hint: Flexbox = flexible boxes).

With flexbox, you can align elements horizontally and vertically. Unlike floats, you can re-order flex items without needing to change the HTML.

## 2. The Flex Model

- `flex` is the value for the display property that activates the Flexbox layout on an element.
- What is a flex container?
- What are flex items?
- What are the most common properties that can be used on a flex container?
  - `flex-direction` (default `row`)
  - `flex-wrap` (default `nowrap`)
  - `justify-content` (default: `flex-start`)
  - `align-items` (default: `stretch`)
  - `align-content` (default: `stretch`)
  - `flex-flow`
- What are the most common properties that can be used on a flex item?
  - `align-self` is similar to `align-items` on the container, but applies to a single flex item.
  - `flex`: shorthand property for the `flex-grow`, `flex-shrink`, and `flex-basis`
  - `flex-grow`: specifies how an item grows when it is allowed to take extra space available in the container (default: 0)
  - `flex-shrink` specifies how an item shrinks when there is not enough space available in the container (default: 1)
  - flex-basis
  - order

# Exercise Description

1. Use Flexbox instead of float to style the navigation bar on the portfolio in [this CodeSandbox](https://codesandbox.io/s/flex1-vkyi2)
2. Use Flexbox to style the HTML form provided in [this CodeSandbox](https://codesandbox.io/s/flexbox2-ymdfj?file=/index.html) (see attached image for expected result)
3. Style the Flexbox Pricing Grid in [this CodeSandbox](https://codesandbox.io/s/flexbox3-w8vqk) (see attached image for expected look)

# Homework

- Bring your website to Checkpoint 13.

# Glossary

- Flexbox - Flexible box

# Resources

- [A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [MDN Flexbox](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)

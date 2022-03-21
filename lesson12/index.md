---
title: Lesson 12 - CSS Layout - Part I
nav_order: 12
---

## Class Agenda

1. Normal Flow
1. The `display` Property
1. Floats

## 1. Normal Flow

This section will help the students to understand how webpage elements are laid out by default.

- Last class introduced the idea that everything on the page is a box.
- By default, these boxes can be stacked up on top of one another, or side by side
- Revision: What does block level and inline elements mean?
- Discuss `display: inline-block`. How is it similar/different to block and inline?

## 2. The `display` Property

You can change how elements behave in normal flow with the `display` property.

Exercise:

1. Apply a border on all elements on your page.
2. Using the dev tools, identify elements with display block and change them to inline (and vice versa)
3. Observe how the flow of elements on the page changes

## 3. Floats

- Float was originally introduced to simple layouts like wrapping text around an image (borrowed from print design).
- But it became used to achieve more complex layouts
- Exercises:
  - We will restructure our HTML a little bit
    - Pull out the `nav` content out of the header, so it is a direct child of the `body`
    - Copy and paste the `nav` across the other HTML files
    - In index.html, the `header` should now be below the `nav` and should contain then `h1` and `img`
    - Check Checkpoint 12 for example with completed steps
  - We will use Float to layout our header contain (logo on the right, navigation bar on the left)
- In the exercises, we'll learn:
  - `float: left`
  - `float: right`
  - Clearing floats

# Exercise Description

Exercises are listed as part of each section.

# Homework

- Checkpoint 12

# Resources

- [Normal Flow](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Normal_Flow)
- [CSS Display Property](https://www.w3schools.com/cssref/pr_class_display.asp)
- [CSS Display](https://developer.mozilla.org/en-US/docs/Web/CSS/display)

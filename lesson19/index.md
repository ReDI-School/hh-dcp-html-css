---
title: Lesson 19 - CSS Selectors II
nav_order: 19
---

# CSS Selectors II

This lesson teaches various CSS Selectors which are not so often used but still important. The theory would be accompanied with practical examples for each selector case.

## Class Agenda

1. Recap of the CSS Selectors I
2. CSS Combinator Selectors
3. CSS Pseudo-classes
4. CSS Pseudo Elements
5. CSS Attribute Selectors

# 1. Recap of the CSS Selectors I

We have written a decent amount of CSS rules for our website so far. While the amount of CSS rules is high, we have not used too many different CSS Selectors for our rules. We have mainly used the Simple CSS Selectors such as

- the CSS element Selector
- the CSS id Selector
- the CSS class Selector
- the CSS universal Selector
- and others

We have covered those selectors during our [introduction CSS lecture](https://redi-school.github.io/nrw-html-and-css/lesson7/#3-css-selectors-i). Apart from that, we have also covered the CSS Descendant Selector which belongs to the group of Combinator Selector during another one of our [CSS lectures](https://redi-school.github.io/nrw-html-and-css/lesson8/#1-css-descendant-selector). The main goal of this lesson is to cover the rest of the CSS Selectors, so that the we learn more possibilities to style our websites.

# 2. CSS Combinator Selectors

A CSS selector can contain more than one simple selector. Between the simple selectors, we can include a combinator.

There are four different combinators in CSS:

- descendant selector (space)
- child selector (>)
- adjacent sibling selector (+)
- general sibling selector (~)

# 3. CSS Pseudo-classes

A pseudo-class is used to define a special state of an element.

For example, it can be used to:

- Style an element when a user mouses over it
- Style visited and unvisited links differently
- Style an element when it gets focus

We have worked with some of these during our [CSS Links and Lists Lesson](https://redi-school.github.io/nrw-html-and-css/lesson9/)
The most important pseudo-classes which this section covers are:

- `:first-child`
- `:last-child`
- `:nth-child()`

If times allow it we would cover some additional pseudo-classes.

# 4. CSS Pseudo Elements

Apart from pseudo-classes there are also pseudo-elements which can be styled with a certain CSS Pseudo-elements Selectors. A CSS pseudo-element is used to style specified parts of an element. For example, it can be used to:

- Style the first letter, or line, of an element
- Insert content before, or after, the content of an element

The most important Pseudo-elements we would cover are:

- `::first-line`
- `::first-letter`
- `::before`
- `::after`
- `::selection`

# 5. CSS Attribute Selectors

It is possible to style HTML elements that have specific attributes or attribute values. This section covers how to do that.

# Glossary & Terminology

- `Pseudo-class` - A CSS pseudo-class is a keyword added to a selector that specifies a special state of the selected element(s). For example, `:hover` can be used to change a button's color when the user's pointer hovers over it.
- `Pseudo-element` - A CSS pseudo-element is a keyword added to a selector that lets you style a specific part of the selected element(s). For example, `::first-line` can be used to change the font of the first line of a paragraph.

# Homework

- Look in your project and review CSS selectors. Think about cases where you can use a different CSS Selector version so that you decrease the number of CSS rules you use and make your CSS file more structured and maintainable.
- In [Checkpoint 19](https://github.com/ReDI-School/nrw-html-and-css/tree/checkpoint19), we have changed some CSS rules definition to show you how different selectors can make more sense in some cases. Please take inspiration from it for your personal project.
  - [What has changed between Checkpoint 19 and Checkpoint 18?](https://github.com/ReDI-School/nrw-html-and-css/compare/checkpoint18...checkpoint19). Use this link to see the differences between two checkpoints. The green highlight (#e5ffec) shows the things which are added with Checkpoint 19.
- Practice your selector skills with this game: ["CSS Diner - the fun way to practice selectors"](http://cssdiner.com). Share a screenshot of your completed levels in the Classroom channel.

# Resources

- [Attribute Selectors](https://www.w3schools.com/css/css_attribute_selectors.asp)
- [Categorization of CSS Selectors](https://www.w3schools.com/css/css_selectors.asp)
- [Combinator Selectors](https://www.w3schools.com/css/css_combinators.asp)
- [Pseudo-classes](https://www.w3schools.com/css/css_pseudo_classes.asp)
- [Pseudo-elements](https://www.w3schools.com/css/css_pseudo_elements.asp)

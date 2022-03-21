---
title: Lesson 16 - CSS Overflow and Text Effects
nav_order: 16
---

# CSS Overflow and Text Effects

## Class Agenda

1. CSS Overflow
2. CSS Text Effects
3. CSS White Space

# 1. Overflow

There are many scenarios in which the content of an html tag is simply bigger than the size of the html tag container itself. This makes the content overflow.

Students would learn about the default `overflow` behaviour and the principle which CSS applies to ["avoid data loss"](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Overflowing_content#css_tries_to_avoid_data_loss).

Apart from that, the section covers the CSS `overflow` property. Students would learn about the different values possible to be added to overflow:

- `visible`
- `hidden`
- `clip`
- `scroll`
- `auto`

Furthermore, this section covers the different directions an overflow can happen. These are `overflow-x` and `overflow-y`. Additionally, the students would learn the requirements for the `overflow` property to work properly. All of this would be taught with practical examples.

ETA: 40 min

# 2. Text Effects

What should we do when we have long words? Should we use scrolling with `overflow-x` ? In this section students would learn alternative and perhaps better approaches to deal with the former problem. This includes covering the [CSS Text Effects](https://www.w3schools.com/css/css3_text_effects.asp) and the respective CSS rules associated with them. These are:

- `text-overflow`
- `overflow-wrap` (`word-wrap`)
- `word-break`
- `line-break`
- `writing-mode`

Some of these rules are very similar but yet distinct enough. The lecture would cover in details the differences between:

- `word-break: break-all` versus `overflow-wrap: break-word` in CSS
- `word-wrap` and `overflow-wrap`
- `line-break` and `word-break`

ETA: 40min

# 3. CSS White Space

Apart from all the above CSS rules there is one additional one which also deals with how content is displayed inside a container. This section teaches the CSS `white-space` rule.

ETA: 20min

---

# Homework

1. The usage of overflow and text effects is more situational. Please practice using these rules on W3Schools or MDN. You can find examples to practice on the respective pages there.

2. Try to make the menu items (links) in the navigation bar of your website scrollable on the horizontal axis when the page is viewed on a very small screen width. This feature is the new thing which we add with checkpoint 16. Here are the respective links to compare your solution

   - [Portfolio Project - Checkpoint 16](https://github.com/ReDI-School/nrw-html-and-css/tree/checkpoint16/checkpoint)
   - [What has changed between Checkpoint 16 and Checkpoint 15?](https://github.com/ReDI-School/nrw-html-and-css/compare/checkpoint15...checkpoint16). Use this link to see the differences between two checkpoints. The right side shows the things which are added with Checkpoint 16.

3. Read the following [article](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Sizing_items_in_CSS) which is a recap of different ways to size items in CSS

Make sure to ask questions!

# Resources

- [How to create a horizontal scrollable menu?](https://www.w3schools.com/howto/howto_css_menu_horizontal_scroll.asp)
- [How to deal with long words?](https://justmarkup.com/articles/2015-07-31-dealing-with-long-words-in-css/)
- [MDN CSS Overflowing Content Tutorial](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Overflowing_content)
- [MDN CSS Overflow rule](https://developer.mozilla.org/en-US/docs/Web/CSS/overflow)
- [MDN White Space rule](https://developer.mozilla.org/en-US/docs/Web/CSS/white-space)
- [W3S CSS Text Effects](https://www.w3schools.com/css/css3_text_effects.asp)

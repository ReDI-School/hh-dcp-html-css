---
title: Lesson 22 - Responsive Design
nav_order: 22
---

In this lesson, we will learn the basics of responsive web design. This is a fundamental concept in the modern web development and deserves special attention.

## Agenda

1. Introduction
2. Dev Tools inspection
3. The viewport meta tag
4. Flexbox behaviour
5. Media Queries

## 1. Introduction

Responsive web design is about creating web pages that look good on all devices! A responsive web design will automatically adjust for different screen sizes and viewports. That is achieved by using such HTML and CSS that makes the web elements shrink, resize or enlarge themselves on different screen sizes. It is important to understand that responsive web design isn't a separate technology — it is a term used to describe an approach to web design or a set of best practices, used to create a layout that can respond to the device being used to view the content. These approaches can include

- Making containers fluid by setting `max-width: 100%`
- Using relative units for typography
- Using CSS Flexbox or CSS Grid to create responsive layouts
- Using media queries to change styles on different viewports

## 2. Dev Tools inspection

It is extremely important to look at the result of your implementation directly in the browser. As you have already learned, the browser Dev Tools are an excellent way to check and debug your html and css code. What's more the browser Dev Tools allow you to check how your page is going to look on different devices such as tablets or mobile phones. Sometimes you can even select from a few built-in device sizes. Use the Dev Tools to check out how your website looks on mobile devices.

## 3. The viewport meta tag

One of the first steps towards responsive design is setting a special HTML meta tag inside the head of your html file.

```html
<meta name="viewport" content="width=device-width,initial-scale=1" />
```

The story behind why this line is needed is very interesting and is worth reading [here](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design#the_viewport_meta_tag).

## 4. Flexbox behaviour

We learned about flexbox in [lecture 14](https://redi-school.github.io/nrw-html-and-css/lesson13/). One of the key aspects associated with flexbox is that it is very useful for responsive designs. This is because the flex items will shrink and distribute space between the items according to the space in their container, as their initial behavior. By changing the values for `flex-grow` and `flex-shrink` you can indicate how you want the items to behave when they encounter more or less space around them.

## 5. Media queries

Responsive design was only able to emerge due to the media query. Media Queries allow us to run a series of tests (e.g. whether the user's screen is greater than a certain width, or a certain resolution) and apply CSS selectively to style the page appropriately for the user's needs.

```
@media screen and (min-width: 800px) {
  .container {
    margin: 1em 2em;
  }
}
```

# Glossary & Terminology

- `Responsive Web Design` - Responsive web design (RWD) is an approach to web design that makes web pages look well on a variety of devices and window or screen sizes from minimum to maximum display size. More info [here](https://en.wikipedia.org/wiki/Responsive_web_design).

# Homework

1. Open the browser dev tools and checkout how your website looks on mobile devices.
2. Identify places which can look bad and try to use the learned techniques to make them look better. If you have difficulties, feel free to ask around for help. Meanwhile checkout our [Checkpoint 22](https://github.com/ReDI-School/nrw-html-and-css/tree/checkpoint22/checkpoint) to get some inspiration and look at examples of what you can do.
3. (Optional) Learn about a more advanced layout concept called [CSS Grid](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout). The CSS Grid is very useful for responsive design but it can be more difficult to master.

# Resources

- [MDN Responsive Design](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design)
- [W3S Responsive Design](https://www.w3schools.com/html/html_responsive.asp)

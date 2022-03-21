---
title: Lesson 21 - Exercise Class III (URL Hash and Icons)
nav_order: 21
---

In this lesson, we will look at some useful techniques such as adding CSS Icons to your website or supplying a hash value to URLs. We would practice the latter directly on your websites. Apart from this we would make sure that you reach the latest Checkpoint 21 and if the time allows we would also do some extra exercises.

## Prerequisite

Every student who enters the class should bring their implementation of their own portfolio project. In other words, every student should bring their code and show it to teachers, ideally in CodeSandbox or locally in their VS Code environment.

## Agenda

1. URL Fragment (URL Hash)
2. CSS Icons
3. Reach [Checkpoint 21](https://github.com/ReDI-School/nrw-html-and-css/tree/checkpoint21/checkpoint)
4. Do extra exercises

## 1. URL Fragment (URL Hash)

The fragment identifier introduced by the hash mark `#` is the optional last part of a URL for a document. It is typically used to identify a portion of that document. It is often very useful to navigate to a certain part in the page without the need to scroll. The `#` hash value can be a special built-in one such as `top` or `bottom`, respectively marking the top and the bottom of the page. Nevertheless, the value of the URL Fragment `#` can be anything you like. Let's try to do an exercise together to see how it in action.

_Exercise:_

- Give each each section of your main page a unique `id`
- Create navigation links which point to sections of your main page
- Apply the following CSS so that the fixed height of your navigation bar is taken into account. More info [here](https://css-tricks.com/almanac/properties/s/scroll-padding/)

```css
html {
  /*
   * This height needs to be the same as the navigation bar height
   * More on this here https://css-tricks.com/almanac/properties/s/scroll-padding/
   */
  scroll-padding-top: 50px;
}

/*
This sets a smooth scrolling behavior when scrolling is triggered by the navigation
Read more here: https://developer.mozilla.org/en-US/docs/Web/CSS/scroll-behavior
*/
* {
  scroll-behavior: smooth;
}
```

## 2. CSS Icons

Icons can easily be added to your HTML page by using an icon library. This is the simplest way and does not require a lot of work. Some famous libraries are

- [Font Awesome](https://fontawesome.com/v6.0)
- [Google Fonts](https://developers.google.com/fonts/)

Every font library contains instructions on how to add fonts or icons to your page. Generally, this happens by attaching a script link to your HTML page such as:

```html
<link
  rel="stylesheet"
  href="https://fonts.googleapis.com/icon?family=Material+Icons"
/>
```

Then if we want to use some icon we only have to add the name of the specified icon class to any inline HTML element (like `<i>` or `<span>`). For example:

```html
<i class="material-icons">cloud</i>
```

All the icons in the icon libraries can be customized with additional CSS (size, color, shadow, etc.)

_Exercise:_

- Add the google font icons library to your website with

```html
<link
  href="https://fonts.googleapis.com/icon?family=Material+Icons"
  rel="stylesheet"
/>
```

> You can also use the Font Awesome library but it requires a personal registration their website. Please go their website and follow the instructions if you would like to access a bigger set of icons

- Change the footer of your website to contain icons from the google font icon library. Check the code in [Checkpoint 21](https://github.com/ReDI-School/nrw-html-and-css/tree/checkpoint21/checkpoint) to see how to do that

## 3. Reach checkpoint 21

Another goal of this class is to make sure that students reach [Checkpoint 21](https://github.com/ReDI-School/nrw-html-and-css/tree/checkpoint21/checkpoint). We would also pay special attention to the implementation of the [background image](https://redi-school.github.io/nrw-html-and-css/lesson20/) in students personal project.

## 4. Extra exercises

If there is enough time we can also do all exercises from the previous exercise classes, i.e. [Exercise Class I](https://redi-school.github.io/nrw-html-and-css/lesson14/) and [Exercise Class II](https://redi-school.github.io/nrw-html-and-css/lesson18/), which we have not managed to cover.

# Homework

Consider looking at the CSS Icons and fonts made available by https://fontawesome.com/. Make yourself familiar with the process of integrating that external library into your project. Try to find places where it would make sense to add icons or use a different font from the ones given by the library.

# Resources

- [CSS Scroll Padding](https://css-tricks.com/almanac/properties/s/scroll-padding/)
- [Google Fonts](https://developers.google.com/fonts/)
- [Font Awesome](https://fontawesome.com/v6.0)
- [MDN Scroll Behaviour](https://developer.mozilla.org/en-US/docs/Web/CSS/scroll-behavior)

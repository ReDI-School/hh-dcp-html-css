---
title: Lesson 20 - CSS Background & Color Values
nav_order: 20
---

# CSS Background & Color Values

In previous classes, we applied flat fill colors (e.g `red`, `#ccc`) as the background on elements,
but CSS gives us a lot more options and effects that we can apply on backgrounds.

In this lesson, we will look at the other effects that CSS allows us to apply on element backgrounds.

## Class Agenda

1. Recap
1. Background Images
1. Background Gradients
1. Background-blend-mode
1. Opacity
1. Gradient generators
1. Other CSS Color Values

## 1. Recap

We have used styles like `background: green` to specify only background colors, but take note that
the `background` property is a shorthand property that is capable of setting not just
the background color, but also [background image, size and other properties](https://developer.mozilla.org/en-US/docs/Web/CSS/background#constituent_properties).

So, when we write `background: green`, it is similar to writing `background-color: green`.

## 2. Background Images

The `background-image` property is used to apply a graphic (e.g JPG) or gradient to the background of an element.
The url() keyword lets you provide the location of the image. See different examples below:

```css
.celebrate {
  background-image: url(balloons.jpg);
}

body {
  background: url(sweet_texture.jpg);
}

.section {
  background: no-repeat url("../../media/examples/lizard.png");
}
.fancy {
  /* You can also set multiple images */
  background-image: url("sparkles.png"), url("balloons.jpg");
}
```

## 3. Background Gradients

You can use CSS to create a gradient with different colors and apply that as a background image.
There are different types of gradients available, e.g. radial, linear, repeating. See examples below.

```css
div {
  background: radial-gradient(black, red);
}

p {
  background: linear-gradient(45deg, black, transparent);
}

.comic {
  background-image: conic-gradient(#ff8, #e71);
}

.gradient {
  background-image: repeating-linear-gradient(
    45deg,
    #af002d,
    #131417 10px,
    #373c49 10px,
    #6d2ee5 20px
  );
}
```

## 4. Gradient generators

There are websites that makes it easy to create gradients, like <https://cssgradient.io/>
Some websites also provide interface to generate the code for other CSS properties e.g <https://html-css-js.com/css/>.

ETA: 40 mins

## 5. background-blend-mode

The `background-blend-mode` property is used to determine how a background image should blend with
the element's background color, or blend into other background image(s) on the same element. Available blend-modes include
`multiply`, `overlay` [and many others](https://developer.mozilla.org/en-US/docs/Web/CSS/blend-mode).

One use case is when trying to adjust how an image looks without creating and loading many versions of the image into the page. For example you can adjust the `background-blend-mode` when a user hovers over an image.

```css
.profile {
  background-image: url(building.jpg);
  background-color: blue;
}

.profile:hover {
  background-blend-mode: multiply;
}
```

## 6. Opacity

Opacity is used to specify how transparent an element should be.
The default value of `opacity` is `1`, where there is no transparency.
`0` means completely transparent.

Take note that opacity applies to not just the background of an element.
It also applies to the content of the element like text. So, you have to be careful when using it on elements with text (e.g `p`), as the text may become difficult to read.

```css
div {
  opacity: 0.5;
}
```

ETA: 30 mins

## 7. Other CSS Color Values

In previous classes, we used color keywords like `red`, `tomato`. CSS offers more powerful ways of specifying colors. These include:

- HEX e.g `#663399`
- RGB e.g `rgb(255,0,153)` and RGBA e.g `rgb(255, 0, 153, 100%)`
- HSL e.g `hsl(270,60%,70%)`
- Other Color keywords (`currentcolor`, `inherit`, `transparent`)

ETA: 20 mins

# Homework

Review the changes in [Checkpoint 20](https://github.com/ReDI-School/nrw-html-and-css/tree/checkpoint20/checkpoint) and try them out in your own projects.

Read more about the topics below. You can start with the pages linked, but feel free to search the internet for more about them.

- [CSS Border-Image](https://www.w3schools.com/css/css3_border_images.asp)
- [CSS Box-Shadow](https://developer.mozilla.org/en-US/docs/Web/CSS/box-shadow)
- [CSS Outline](https://www.w3schools.com/css/css_outline.asp)

# Resources

- [A Complete Guide to CSS Gradients](https://css-tricks.com/a-complete-guide-to-css-gradients/)
- [All blend-mode keyword values](https://developer.mozilla.org/en-US/docs/Web/CSS/blend-mode)
- [Basics of CSS Blend Modes](https://css-tricks.com/basics-css-blend-modes/)
- [MDN background property page](https://developer.mozilla.org/en-US/docs/Web/CSS/background)
- [Repeating Gradients Background](https://www.youtube.com/watch?v=muE2B0Zylbw)

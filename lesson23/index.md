---
title: Lesson 23 - CSS Animations & Transitions
nav_order: 23
---

## Agenda

1. Introduction
1. Animations
1. Transitions
1. Transform

## 1. Introduction

An animation lets an element gradually change from one style to another.
You can create nice animations with CSS on properties such as color, background-color, height, or width.
See full list of [Animatable properties](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_animated_properties).
In this lesson, we cover a few CSS properties to achieve animations.

## 2. Animations

The first type of animation we describe below is one that starts immediately when the page loads even without user interaction.
To create this, we need to know about the `animation` property (plus other related properties) and the `@keyframes` rule.

- `animation-name`: Specifies the name of the `@keyframes` rule describing the animation.
- `animation-duration`: Sets the length of time that the animation should take.
- `animation-delay`: Sets a time before the animation starts
- `animation-iteration-count`: Sets the number of times the animation should run
- `animation-timing-function`: Configures the timing or speed of the animation.

Each keyframe rule defines what should happen at specific moments during the animation.
For example, 0% is the start and 100% is the end,

```css
.element {
  height: 200px;
  /* animation-name must match @keyframes value */
  animation-name: pulse;
  animation-duration: 5s;
  animation-iteration-count: infinite;
}

/* @keyframes <animation-name> with <percentage> steps */
@keyframes pulse {
  0% {
    background-color: #001f3f;
  }
  40% {
    background-color: #0e1;
  }
  100% {
    background-color: #ff4136;
  }
}
```

You can also use keywords `from` and `to` with @keyframes.

```css
h1 {
  font-size: 20px;
  animation-name: size-increase;
  animation-duration: 5s;
}

@keyframes size-increase {
  from {
    font-size: 20px;
  }
  to {
    font-size: 80px;
  }
}
```

## 3. Transitions

Transitions are typically applied when a user interacts with an element (e.g when a user hovers or clicks on an element).

- `transition-property`: used to define what property, or properties, you want to apply a transition effect to. You can also use the keyword `all` to transition all properties possible to transition on the element.
- `transition-duration`: used to define the duration of a specified transition.
- `transition-delay`: used to define a length of time to delay the start of a transition
- `transition-timing-function`: used to define a function that describes how a transition will proceed over its duration

```css
div {
  transition: all 0.5s ease;
  background: red;
  padding: 10px;
}

div:hover {
  background: green;
  padding: 20px;
}
```

## 4. Transform

The `transform` property is usually used alongside animations. It allows you to visually manipulate an element by skewing, rotating, translating, or scaling. You can set transform on an element without animations e.g

```css
div {
  width: 20px;
  height: 20px;
  transform: scale(20);
}
```

but works well with transitions and animations e.g

```css
a {
  font-size: 2em;
  transition: transform 0.3s ease-out;
  display: inline-block;
}

a:hover {
  /* this lifts up the link on hover */
  transform: translate(0, -5px);
}
```

# Glossary & Terminology

- `Animatable CSS properties` - List of CSS properties can be animated using CSS Animations or CSS Transitions. More info [here](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_animated_properties).

# Homework

1. Checkout the Checkpoint23 branch and apply similar styles to your project.
2. Learn how to use the shorthand `animation` and `transition` properties. See resources below.

# Resources

- [Animation on MDN Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/animation)
- [Transition property](https://css-tricks.com/almanac/properties/t/transition/)

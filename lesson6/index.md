---
title: Lesson 6 - HTML Forms
nav_order: 6
---

# HTML Forms

## Class Agenda

1. What are HTML Forms?
2. Form Tags (Part 1)
3. Form Tags Part 2 (if there is time)

## 1. What are HTML forms?

- Allow us to get information from users
- Look at examples of forms on other websites
  - Sign up / Log in forms
  - Search Box
  - Contact Form
  - Payment Form

ETA: 20 mins

## 2. Form Tags (Part 1)

- There are many tags needed to make a working form. For now, we will cover a few.

### `<form>`

- All forms start with a `<form>` element. It is a container element like `<section>` but for containing forms.
- Two important attributes of `<form>`:
  - action - defines the location (URL) where the form's collected data should be sent when it is submitted.
  - method - defines which HTTP method to send the data with

### `<input>`

- used to create elements that specifically accept data (input) from the user
- There are different types of input elements

  - `<input type="text">`
  - `<input type="email">`
  - `<input type="password">`
  - `<input type="search">`
  - `<input type="submit">`
  - `<button type="submit">Submit</button>`
  - See other input types [here](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input#input_types)

ETA: 25 mins

### `<label>`

- represents a caption for an item
- importance of adding a `<label>` for an `<input>` element
  - A user can click the label to focus/activate the associated input
  - A screen reader will read out the label when a user interacts with it's input
- the `for` attribute

ETA: 15 mins

### `<textarea>`

- represents a multi-line plain-text editing
- Note: This is not an empty element. It requires a closing tag.

ETA: 10 mins

- Task: Make time for students to try out the introduced tags.
- Task: Show this [image](./form-quiz.png) of a contact form, and let students identify tags to be used for creating it.
- Task: Checkpoint 6:

  - Take a few mins to explain the concept of Checkpoints to the students and how we are using it to build the Portfolio Project, and ensure they are up to date

- Create a "Contact Me" Page for the Portfolio Project.
  - Students are to create a contact form similar to [this](./form-sketch.png)
  - The page should use the introduced tags
  - The students should test that their forms can submit data with both GET and POST methods.

ETA: 40 mins

## Form Tags (Part 2)

**If there's more time left in the class**

- `<input type="checkbox">`
- `<input type="radio">`
- `<select>`
- `<option>`

# Exercise Description

Students should complete Checkpoint 6 as described above.

# Glossary & Terminology

- HTML form - An HTML form is used to collect user input. [Source](https://www.w3schools.com/html/html_forms.asp)

# Homework

- Go over everything we have covered for HTML so far. The next class will be on CSS, so make sure you understand what has been taught so far.
- Review your copy of the Portfolio Project and make sure that you are at a similar structure with Checkpoint 6.
- **(Optional) Bonus Lecture - HTML Tags 3** - If you would like to learn about even more HTML Tags to further increase your HTML knowledge before diving into CSS you can take a look at a bonus lecture material we have composed for you. In this [bonus lecture](https://github.com/ReDI-School/nrw-html-and-css/blob/master/teacher/intermediate_lesson5-7/index.md) you are expected to teach yourself different HTML Multimedia tags and other interesting HTML tags and character entities.

# Resources

- [MDN's HTML Forms Page](https://developer.mozilla.org/en-US/docs/Learn/Forms)

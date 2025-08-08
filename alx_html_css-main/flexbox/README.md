# ALX FLEX BOX PROJECT

## Table Of Content
- [Overview](#overview)
- [Task 0](#task-0)
    -[Add Display Flex](#add-display-flex)
    -[Outcome Of Task 0](#outcome-of-task-0)
- [Task 1](#task-1)
    - [Add New Classes On Section](#add-new-classes-on-section)
    - [Outcome Of Task 1](#outcome-of-task-1)
- [Task 2](#task-2)
    - [Reverse Order Latest News Card](#reverse-order-latest-news-card)
    - [Outcome Of Task 2](#outcome-of-task-2)
- [Task 3](#task-3)
    - [Simplify Service List](#simplify-service-list)
    - [Outcome Of Task 3](#outcome-of-task-3)
- [Task 4](#task-4)
    - [Playing Around With The Spacing Between Flex Service Items](#playing-around-with-the-spacing-between-flex-service-items)
- [Task 5](#task-5)
    - [Flexify The Header](#flexify-the-header)
    - [Outcome Of Task 5](#outcome-of-task-5)
- [Task 6](#task-6)
    - [Flexify The Navbar](#flexify-the-navbar)
    - [Outcome Of Task 6](#outcome-of-task-6)
- [Task 7](#task-7)
    - [Align Center Logo And Navbar](#align-center-logo-and-navbar)
    - [Outcome Of Task 7](#outcome-of-task-7)
- [What I learned](#what-i-learned)
- [Resources](#resources)
- [Author](#author)
## Overview

This is a task project given by ALX introduction to software programme. The task is centered on learning about flex box and how to use it in web development.

The flex box layout is used in css to give the html structure a good layout structure. Adding beauty and aesthetics.

ALX provided the HTML starter files and CSS starter files.

The images used in this project were used as a placeholder on instruction of ALX.

## Task 0

### Add Display Flex

The first task I was asked to:
* Copy the starter files into 0-index.html and 0-styles.css respectively.
* Add a selector for the row class and add the property display with the value of flex in the grid section of the css file.

### Outcome Of Task 0

Here are some of the code used:
```CSS
.row{
    display: flex;
}
```

## Task 1

### Add New Classes On Section

For this task I was asked to:
* Copy the previous task as the base of this task  and rename as 1-index.html and 1-styles.css respectively.
* Add the class `section-services` to the `.service` section tag.
* Add the class `section-works` to the `.works` section tag.
* Add the class `section-about-us` to the `.about` section tag.
* Add the class `section-latest-news` to the `.latest_news` section tag.
* Add the class `section-testimonial` to the `.testimonial` section tag.
* Add the class `section-contact` to the `.contact` section tag.

### Outcome Of Task 1

Here are some of the code used:
```HTML
<section id="services" class="section section-services">
<section id="about" class="section section-about-us">
<section id="latest_news" class="section section-latest-news">
```
## Task 2

### Reverse Order Latest News Card

For this task I was asked to:
* Copy the previous task as the base of this task  and rename as 2-index.html and 2-styles.css respectively.
* Target the `row` class inside `section-latest-news`
* Set the `flex-direction` to `row-reverse`

### Outcome Of Task 2

Here are some of the code used:
```CSS
.section-latest-news .row{
    flex-direction: row-reverse;
}
```

## Task 3

### Simplify service List

For this task I was asked to:
* Copy the previous task as the base of this task  and rename as 3-index.html and 3-styles.css respectively.
* Remove the second `ul` tag in the `service section` of the index.html file and but its `li` elements in the first `ul` tag.
* Target the `row` class inside the `section-service` class.
* Add the property `flex-wrap` with the value `wrap` in the targeted class.

### Outcome Of Task 3

Here is the preview of the outcome.
![Preview of the completed task 3](/flexbox/images/task-3.png)

## Task 4

### Playing Around With The Spacing Between Flex Service Items

For this task I was asked to:
* Copy the previous task as the base of this task  and rename as 4-index.html and 4-styles.css respectively.
* Replace the current width with `calc((100% / 3) - 2rem)` in the `.col-1-3` selector in the 4-styles.css file
* Replace the current width with `calc((100% / 2) - 2rem)` in the `.col-1-2` selector
* Remove the padding declaration and set the `margin` property to `1rem` in the `[class*='col-]` selector.
* Replace the current margin with `-1rem` in the `ul.row` declaration.

### Outcome of Task 4

Here is the preview of the completed task
![Preview of the completed task 4](/flexbox/images/task-4-outcome.png)

## Task 5

### Flexify The Header

For this task I was asked to:
* Copy the previous task as the base of this task and rename as 5-index.html and 5-styles.css respectively.
* In the 5-index.html file, Wrap the div with class `header-logo` and the div with class `navbar-menu` with a div that has `header-container` as a class.
* In the 5-styles.css file,
    * Inside the `/*Header` section, add a selector for the `header-container` class and add the following properties:
        * Property: `display`, Value: `flex`
        * Property: `justify-content`, Value: `space-between`
    * Remove `header-logo` and `header-logo a` rules
    * Remove the `navbar-menu` rule
    * In the variable section, remove
        * header-logo-position
        * header-logo-link-display
        * header-logo-link-position
        * header-logo-link-top
        * header-logo-link-left

### Outcome Of Task 5

Here are some of the code used:
```HTML
  <div class="container">
        <div class="header-container">
```

```CSS
  .header-container{
    display: flex;
    justify-content: space-between;
}
```

## Task 6

### Flexify The Navbar

For this task I was asked to:
* Copy the previous task as the base of this task and rename as 6-index.html and 6-styles.css respectively.
* Add the property `display` with the value `flex` in the `/*Navbar` section of the css file.
* In the same section, remove the display declaration in the `.nav .nav-item` selector.
* Move the margin from the `.nav .nav-item` selector to the targeted `.nav .nav-item` inside the `.nav` class.
* Change the value of the variable `nav-item-margin` to `0 0 0 2rem` in the variable section of the css file.

### Outcome Of Task 6

Here are some of the code used:
```CSS
.nav .nav-item + .nav-item{
    margin: var(--nav-item-margin);
}

.nav {
    display: flex;
}
```

## Task 7

### Align Center Logo And Navbar

For this task I was asked to:
* Copy the previous task as the base of this task and rename as 7-index.html and 7-styles.css respectively.
* set the property `align-items` to `center` in the `header-container` class selector inside the `/*Header` section of the css file.

### Outcome Of Task 7

Here is a snippet of the code:

```CSS
.header-container{
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
```
 
## What I learned
I learned about flex properties like `align-items`, `flex-direction`, `justify-content`, `flex-wrap` etc. and how to apply the properties to html. 

## Resources

These materials helped me get a good understanding of the flexbox layout especially the games.
* [A Complete Guide to Flexbox | CSS-Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
* [Flexbox Froggy - A game for learning CSS flexbox](http://flexboxfroggy.com/)
* [Flexbox Defense](http://www.flexboxdefense.com/)
* [Flexbox Cheatsheet](https://yoksel.github.io/flex-cheatsheet/)
* [CSS Flexible Box Layout - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout)

## Author
Like what you read? You can also connect with me on Twitter - [@obika_viola](https://www.twitter.com/obika_viola)

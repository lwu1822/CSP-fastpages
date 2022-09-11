---
toc: true
layout: post
description: App Lab Planning
categories: [code.org]
title: App Lab Plan
comments: true
---

Here is the [link](https://studio.code.org/projects/applab/dbyn_t-_ioCVUC9PB3UiDjg0mKNmHCLnMy0F5ND1uRY) to my app. 

## Subject

Since I'm in AP Stats, I decided to create a statistics quiz. 

## Questions
1. What is the mean of the following set of numbers: 5, 8, 9, 15, 16?
2. (Normal distribution picture): What percent of data lies between one standard deviation of the mean?
3. A class of 30 students were surveyed on how many hours they sleep. The average was 7 hours with a standard deviation of 1.5 hours. What percentage of students sleep less than 8 hours? 

## Design
My app consists of five screens: Homepage, questions 1-3, and the end screen. 

Below are some pictures of what the initial design looked like:

<img src="https://lwu1822.github.io/CSP-fastpages/images/w3AppLabPlan-appLabOriginalText.jpg" alt="Original homepage" width="143" height="200">

<img src="https://lwu1822.github.io/CSP-fastpages/images/w3AppLabPlan-appLabOriginalAnswer.jpg" alt="Original text" width="140" height="179">

After the initial design, I made a few revisions, namely changing the font, adding buttons (originally, the user had to click the screen), and adding radio buttons for the multiple choice selection. 

An intermediate photo where I added a button: 

<img src="https://lwu1822.github.io/CSP-fastpages/images/w3AppLabPlan-appLabButtonChange.jpg" alt="Button added" width="149" height="207">

One of my screens on the final design: 

<img src="https://lwu1822.github.io/CSP-fastpages/images/w3AppLabPlan-appLabFontChange.jpg" alt="Original text" width="138" height="210">


## Coding

My code is relatively simple. A majority of the code used the `onEvent` function. I used the function for two purposes, the first was to change the screen when the Next button was pressed, and the second was to increase the score if the correct multiple choice was selected. 

### Explanations of code

This is a screenshot of part of my code. The rest of my code followed basically the same format. If you wish to check out my code, you can do so [here](https://studio.code.org/projects/applab/dbyn_t-_ioCVUC9PB3UiDjg0mKNmHCLnMy0F5ND1uRY/view).

<img src="https://lwu1822.github.io/CSP-fastpages/images/w3AppLabPlan-appLabCode.jpg" alt="My AppLab code">

Here's how the code works: 

The first block of code is an `onEvent` function, in which when the next button (`q1ButtonNext`) was pressed, the app screen will change to the next question (`q2Screen`).

The second block of code is another `onEvent` function. This time though, when choice B is selected (`q1ButtonB`), a predefined variable `score` will increase by 1. 


### Things I learned

The code I encountered in AppLab was new to me. I used the documentation [^1] very frequently.

I had to learn most of the things I coded. The most important code that I learned was the `onEvent` function. You can use it to specify an action to do when a certain event occurs, such as the press of a button. 


[^1]: [Documentation 1](https://studio.code.org/docs/ide/applab/expressions/button) and [2](https://studio.code.org/docs/concepts/)
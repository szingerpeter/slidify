---
title       : Slidify project
subtitle    : Developing data products
author      : Peter Sz
job         : Student
framework   : revealjs        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

<!-- Limit image width and height -->
<style type='text/css'>
img {
    max-height: 560px;
    max-width: 964px;
}
</style>

<!-- Center image on slide -->
<script src="http://ajax.aspnetcdn.com/ajax/jQuery/jquery-1.7.min.js"></script>
<script type='text/javascript'>
$(function() {
    $("p:has(img)").addClass('centered');
});
</script>

## General description

The shiny application developed calculates the linear model, which best fits the given X and Y variables. 

Then, the fitted model is represented in two ways, as a plot and as a text output.

--- .class #id 

## Input

The application takes two inputs, X and Y values.

Note:
- They must be both numbers, separated by ',' (commas).
- They must have the same length.

E.g.: the input:
- X values: 1, 2, 4
- Y values: 3, 5, 6

will fit the points: (1,3), (2,5), (4,6)

--- .class #id 

## Output

1. Fitted linear model:
  - Intercept: The intercept of the fitted linear model.
  - Slope: The slope of the fitted linear model.

2. Plot:
The plot represents the points given by the user and the fitted linear model.

--- .class #id 

## Example
The input:
- X values: 1, 2, 3
- Y values: 2, 3, 4

Will create the plot:

![plot of chunk unnamed-chunk-1](figure/unnamed-chunk-1-1.png)

--- .class #id 

## Application UI

This is how the application looks like when it's running:

<div style='text-align: center;'>
    <img height='560' src='https://raw.githubusercontent.com/szingerpeter/Peter-Sz/master/shiny.jpg'/>
</div>

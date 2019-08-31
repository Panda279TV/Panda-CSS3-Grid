# Pandas CSS3 Grid System
### I have tried many grid systems or grid frameworks. Many were too big or too confusing. That's exactly why I wrote my own CSS Grid. It is minimalistic, super simple and has only the most important functions. 

### To use this grid, you just have to include the following link in the Head Tag. Link the Author!

Example:

`<!-- Copyright (c) 2019 Benedikt Wolf https://github.com/Panda279TV -->`

`<link rel="stylesheet" href="pandas-grid.css">`

`<link rel="stylesheet" href="YOUR.CSS.FILE">`

---

## Demo

![](pandas-grid-demo.gif)

The [DEMO](https://github.com/Panda279TV/Panda-CSS3-Grid/blob/master/pandas-grid-demo.gif) shows the [HTML FILE](https://github.com/Panda279TV/Pandas-CSS3-Grid/blob/master/pandas-grid-test.html). You can download this and the CSS and have a look at it again.

---

## Statistics
- Minimalistic and Small
- Simple, Easy and Fast to learn
- Normal or Responsive Grid
- Very good and practical grid Padding distances (row = padding: 1% 2%;) (col = padding: 1%;)
- No CSS `!Important`
- Only about 2200 kilobytes (pandas-grid.min.css)
- Works with older browsers (-webkit, -moz, -ms)

---

## First Step

#### The Media Queries Grid will only work if this line has been included in the Head Tag of the HTML Structure! The meta name="viewport".

The class s- works without media queries to create an important prerequisite. The other m-, l-, xl-, .container work only with media queries and therefore you have to integrate the Meta Viewport. Otherwise you couldn't write any media queries yourself!

`<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">`

[Learn more about Media Queries and the Meta Name Viewport!](https://github.com/Panda279TV/CSS3-Media-Queries)

---

## Introduction

My Grid has 12 columns. No matter the size of the browser, each of these columns will always have an equal width.

Each column is width: 8.3333333333333333333%, that result then times 12 gives the width: 100%.

Because of padding distances, these columns do not touch each other with their content and even at 100% the content will not touch the pages left and right!

#### In order to use the grid correctly, a row must be around a column!

    <div class="row">
      <div class="col s-1">1</div>
      <div class="col s-1">2</div>
      <div class="col s-1">3</div>
      <div class="col s-1">4</div>
      <div class="col s-1">5</div>
      <div class="col s-1">6</div>
      <div class="col s-1">7</div>
      <div class="col s-1">8</div>
      <div class="col s-1">9</div>
      <div class="col s-1">10</div>
      <div class="col s-1">11</div>
      <div class="col s-1">12</div>
    </div> 

---

## Container
The container class is not strictly part of the grid but is important in laying out content. It allows you to center your page content. The container class is set to 70% of the window width (responsive 70% to 90%). It helps you center and contain your page content. I use the container to contain my body content.

To add a container just put your content inside a `<div>` tag with a container class. Here's an example of how your page might be set up.
  
    <div class="container">
      <!-- Page Content goes here -->
    </div> 

---

## Responsive Layouts
Above i showed you how to layout elements using my grid system. Now i show you how to design your layouts so that they look great on all screen sizes.

Screen Sizes

| Table       | Mobile Devices <= 600px | Tablet Devices > 601px | Desktop Devices > 992px | Large Desktop Devices > 1281px |
|:------|:------:|:------:|:------:|:------:|
| Class Prefix | .s- | .m- | .l- | .xl- |
| Number of Columns | 12 | 12 | 12 | 12 |
| Container Width | 90% | 83% | 76% | 70% |

Adding Responsiveness
In the previous examples, i only defined the size for small screens using "col s-12". This is fine if i want a fixed layout since the rules propagate upwards.

By just saying s-12, we are essentially saying "col s-12 m-12 l-12 xl-12". But by explicitly defining the size we can make our website more responsive.

---

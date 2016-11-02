# Exam: HTML & CSS

### Getting Started
 - Fork this repository under your own account
 - Commit your progress frequently and with descriptive commit messages
 - All your answers and solutions should go in this repository

### What can I use?
 - You can use any resource online, but **please work individually**
 - Instead of copy-pasting your answers and solutions, write them in your own words.


# Tasks

## 1. Build a design (~90 minutes) [10 points]
Build the following profile cards according to the design provided.   
Follow the design as closely as possible.   
Commit an HTML and a CSS file to this repository.
![design](exercise-1.png)

### Assets
John Duck | Jane Duck | Pencil icon
--------- | --------- | -----------
![duck](duck.jpg) | ![duck](duck2.jpg) | ![pencil-icon](edit-icon.png)   

### Other data
  - Name font size: 28 pixels
  - Text size: 14 pixels
  - Font family: Arial, sans-serif

### Acceptance criteria
The task is accepted if:
  - The result follows design [2p]
  - The code follows style guide [1p]
  - The CSS & HTML are valid [1p]
  - The HTML considers semantic responsibilities [2p]
  - The code avoids code duplication [2p]
  - The CSS has meaningful and short selectors [2p]

Extra points for if:
  - the result is centered on the page [2p]


## 2. Understand code (~15 minutes) [2 points]
Read the following code snippet:   
What is the distance between the top-left corner of the document body and the yellow box?   
Give a detailed explanation below!   
Add your answer to this readme file, commit your changes to this repository.
```HTML
<!DOCTYPE html>
<html>
  <head>
    <style>
      body {
        padding: 0px;
        margin: 0px;
      }
      .foo {
        top: 20px;
        left: 20px;
        width: 100px;
        height: 100px;
        position: absolute;
        background: blue;
      }
      .bar {
        top: 20px;
        left: 20px;
        width: 30px;
        height: 30px;
        position: absolute;
        background: yellow;
      }
    </style>
  </head>
  <body>
    <div class="foo">
      <div class="bar"></div>
    </div>
  </body>
</html>
```

It's 40 px, because their positions are absolute; the body has no padding or margin, and the .foo is 20 px from the body + the .bar is 20 px from the foo (top-left).

## 3. Explain concepts (~15 minutes) [4 points]

Add your answer to this readme file, commit your changes to this repository.

### Explain the difference between `display: block` and `display: inline` in CSS! What is `display: inline-block`?

Every element on  website is a box, and the display property tells them how to behave. When using display:block it generates an inline element box. Block elements are usually conatiners, and don't stay inline. Block is a basic value, so a lot of elements are set to this by default. Without setting the width they take up all the space horizontally.
Display:inline is the default value for all elements. Inline elements accept margin and padding, but ignore width and height.
Display:inline-block is almost the same as display:inline, but you can set width and height to these elements.

### What is the difference between a `<section>` and an `<article>` element? Name one good example of using an `<article>`.

Article tags stand for self-contained, individual content. These can be blog/forum posts, articles, entries, etc. An article element should be indentified, and able to stand on its own, independently from other elements.
The section tag defines sections of a document. Like article tags, sections should be indentified  too.


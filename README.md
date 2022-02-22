# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![images/screenshot.png]

### Links

- Solution URL: [https://github.com/naufalf25/nftpreviewcard]
- Live Site URL: [https://naufalf25.github.io/nftpreviewcard/]

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties

### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>NFT Preview Card Component</title>
    <link rel="stylesheet" href="style.css" type="text/css">
  </head>
  <body>
    <div class="card">
      <div class="head">
        <figure>
          <a href="#"><img src="images/image-equilibrium.jpg" alt="equilibrium"></a>
        </figure>
      </div>
      <div class="middle">
        <img src="images/icon-view.svg" alt="view">
      </div>
      <div class="text">
        <div id="head-text">
          <a href="#"><h1>Equilibrium #3429</h1></a>
          <p>Our Equilibrium collection promotes balance and calm</p>
        </div>
        <div id="foot-text">
          <div class="float-left">
            <p><img src="images/icon-ethereum.svg" alt="ethereum" width="10px">0.041 ETH</p>
          </div>
          <div class="float-right">
            <p><img src="images/icon-clock.svg">3 days left</p>
          </div>
        </div>
        <div class="line"><hr></div>
        <div class="profile">
          <p><img src="images/image-avatar.png" alt="avatar" width="30px">Creation of <a href="#"><span class="cyan">Jules Wyvern</span></a></p>
        </div>
      </div>
    </div>
  </body>
</html>
```
```css
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    background-color: hsl(217, 54%, 11%);
}

.card {
    width: 300px;
    height: 510px;
    background-color: hsl(216, 50%, 16%);
    position: absolute;
    left: 50%;
    right: 50%;
    top: 50%;
    bottom: 50%;
    margin-right: -50%;
    transform: translate(-50%, -50%);
    border-radius: 15px;
}

.card figure {
    margin: 20px;
    border-radius: 10px;
    border: 270px;
    background-color: cyan;
}

.card figure img {
    opacity: 1;
    width: 100%;
    border-radius: 10px;
    -webkit-transition: 0.5 ease-in-out;
    transition: 0.5 ease-in-out;
}

.card figure:hover img {
    opacity: 0.5;
}

.head img:hover .middle img {
    opacity: 1;
}

.middle {
    opacity: 0;
    position: absolute;
    left: 42.5%;
    top: 25%;
}

@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600&display=swap');

.text {
    font-family: 'Outfit', sans-serif;
    padding: 0 20px;
}

#head-text h1 {
    color: white;
    font-weight: 600;
    font-size: 20px;
    margin-bottom: 15px;
}

#head-text a {
    text-decoration: none;
}

#head-text h1:hover {
    color: cyan;
}

#head-text p {
    color: hsl(215, 51%, 70%);
    font-size: 15px;
    font-weight: 300;
}

#foot-text p {
    font-size: 13px;
    font-weight: 500;
    margin: 20px 0;
    overflow: hidden;
    text-overflow: ellipsis;
}

.float-left p {
    color: cyan;
    float: left;
    width: 50%;
}

#foot-text img {
    margin-right: 7px;
    vertical-align: middle;
}

.float-right p {
    color: hsl(215, 51%, 70%);
    float: right;
    width: 50%;
    text-align: right;
}

hr {
    width: 100%;
    background-color: hsl(215, 32%, 27%);
    border: 0;
    border-top: 1px solid hsl(215, 32%, 27%);
}

.profile {
    margin: 15px 0;
}

.profile p {
    color: hsl(215, 51%, 70%);
    font-weight: 400;
    font-size: 14px;
}

.profile img {
    vertical-align: middle;
    border: 1px solid white;
    border-radius: 50%;
    margin-right: 15px;
}

.cyan {
    color: white;
}

.profile .cyan:hover {
    color: cyan;
}

.profile a {
    text-decoration: none;
}
```

### Useful resources

- [https://w3schools.com] - This helped me to get reference about styling.

## Author

- Frontend Mentor - [https://www.frontendmentor.io/profile/naufalf25]
- Instagram - [https://www.instagram.com/naufal_railfans25/]

# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
    - [Desktop](#desktop)
    - [Mobile](#mobile)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

#### Desktop
![](../images/screenshot_desktop.png)

#### Mobile
![](../images/screenshot_mobile.png)


### Links

- [Solution URL](https://github.com/Risclover/stats-preview-card)
- [Live Site URL](https://risclover.github.io/stats-preview-card/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

#### Layout
I started out by turning the HTML into a layout that I thought could work. Since I'm getting pretty used to CSS Flexbox now, I was able to think about it for a moment and then execute it, which I'm happy about! Flexbox used to confuse me, but I think I've conquered it.

I looked at the challenge picture (of what the page should look like when finished) and decided to do the following within the body tags:

```html
<main>
<!-- Main container -->
<div id="main"> 

  <!-- Left side of main container -->
  <div id="left"> 

    <!-- Main text on upper left side -->
    <div id="maintext">
      <h1>
        Get <span class="highlight">insights</span> that help your business grow.
      </h1>

      <p>
        Discover the benefits of data analytics and make better decisions regarding revenue, customer 
        experience, and overall efficiency.
      </p>
    </div>

    <!-- Stats on lower left side -->
    <div id="stats">
      <div class="statsbox">
        <h2>10k+</h2> <p class="stathead">companies</p>
      </div>

      <div class="statsbox">
        <h2>314</h2> <p class="stathead">templates</p>
      </div>

      <div class="statsbox">
        <h2>12M+</h2> <p class="stathead">queries</p>
      </div>
    </div>

  </div>

  <!-- Right side of main container -->
  <div id="right">
    <img src="images/image-header-desktop.jpg" alt="Business women">
  </div>
</div>
<!-- Footer credits -->
<div class="attribution">
  Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
  Coded by <a href="#">Risclover</a>.
</div>
</main>
```

#### Making My Page Responsive
I am extremely excited because I was able to make this website pretty much totally responsive. It was my first time using two media queries to do so, after figuring out that ~710px was the spot where I needed to make that sort of switch from mobile to desktop (through manual testing).

```css
@media screen and (min-width: 711px){

...

}
```

```css
@media screen and (max-width: 710px) {

...

}
```

The thing is, the Challenge gives you a few parameters to use - for example, 15px for the main font. But I wasn't able to make my page fully responsive until I got rid of all of the px and made pretty much most of my units vw instead. Go look at my CSS code for yourself to see what I mean.

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
